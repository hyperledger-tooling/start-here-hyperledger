---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2247" class=".btn">#2247</a>
            </td>
            <td>
                <b>
                    chore!: drop python 3.6 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update setup.py minimum python version requirement.
Update workflows to use Python 3.9 by default.
Update container image docs.

@swcurran @WadeBarnes I believe these are the relevant changes in workflows and setup files in order to officially drop Python 3.6. I think once we've made the transition, there are a number of dependencies that ought to be updated. I think those updates are best suited to a follow up PR.

closes: #2244 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 20:01:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2246" class=".btn">#2246</a>
            </td>
            <td>
                <b>
                    Upgrade codegen tools in `scripts/generate-open-api-spec` and publish Swagger 2.0 and OpenAPI 3.0 specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now is as good a time as any to upgrade the codegen tools in `scripts/generate-open-api-spec` to use the latest `swaggerapi/swagger-codegen-cli` release (it was ~3 years out of date). 

Additionally, I added the latest `openapitools/openapi-generator-cli`, so that the spec generation now provides both a Swagger 2.0 spec, and an OpenApi 3.0 spec. This way users don't need to manually upgrade the spec themselves.

Previously the Swagger 2.0 spec was simply called `openapi.json`. This is now renamed `swagger.json`, with the 3.0 compatible spec in its place. 

Worth noting that the spec validation still only throws warnings that can be ignored:
- the `swagger` spec validation only complains about some missing operationId's (and 'host' not defined);
- and the `open-api` spec validation only complains about `example` fields being unexpected, and a single case of `attribute tags.tagsexternalDocs.url is missing`.

Also, I updated the `UsingOpenAPI.md` file to reflect these changes, with some minor neatening up included.

Review can be validated by running `scripts/generate-open-api-spec`.

Discussion re further edits is welcome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 12:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2245" class=".btn">#2245</a>
            </td>
            <td>
                <b>
                    ./run_demo performance -c 1 --mediation --timing --trace-log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bug with prompt_toolkit and trace logging. Could only bump up the prompt_toolkit library so much since demos run on Python 3.6. However, I did attempt on 3.9 with the latest version of prompt_toolkit and setting an env var (see https://github.com/prompt-toolkit/python-prompt-toolkit/pull/898). This still did not correct the issue, so reverted to existing code and just handled the exception(s). The output of the trace log is being written to the console, my limited understanding of this would be that the trace log works, but also triggers the prompt_toolkit to do the same work and gets into conflict.

Fixes #2205 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 17:21:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2243" class=".btn">#2243</a>
            </td>
            <td>
                <b>
                    fix: route multitenant connectionless oob invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This addresses an issue where the keys used in connectionless oob invitations were not correctly set-up for routing through the base wallet when multi-tenancy is enabled, which resulted in those invitation not being usable.

cc @lohanspies @ff137


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 12:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2241" class=".btn">#2241</a>
            </td>
            <td>
                <b>
                    Feat: Added support for Ed25519Signature2020 signature type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 15:37:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2240" class=".btn">#2240</a>
            </td>
            <td>
                <b>
                    fix: only cache completed connection targets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjusts the caching behavior for connection targets to solve some issues seen in multi-replica setups under certain circumstances.

### The Problem

Given the following conditions,
- ACA-Py is connecting to a remote agent through the remote agent's Public DID
- ACA-Py is using more than one replica with loadbalancing such that one replica may start a DID Exchange/Connection and another may finish the exchange.
- Following connection, ACA-Py attempts to issue a credential to the remote agent (or theoretically any other message where the protocol requires a connection)

If the agent that initiates the credential issuance is not the same agent that completed the DID exchange, the agent will have a connection target cached that still contains the public DID and public routing info of the remote agent, causing the remote agent (if it's also running ACA-Py) to get errors like the following:

```
2023-05-23 18:18:55,358 aries_cloudagent.core.conductor ERROR Exception in message handler:
Traceback (most recent call last):
  File "/usr/lib/python3.9/asyncio/tasks.py", line 256, in __step
    result = coro.send(None)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/core/dispatcher.py", line 264, in handle_message
    await handler(context, responder)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/protocols/issue_credential/v2_0/handlers/cred_offer_handler.py", line 51, in handle
    raise HandlerException(
aries_cloudagent.messaging.base_handler.HandlerException: No connection or associated connectionless exchange found for credential offer
```

This is because it received a message encrypted for it's public DID and key, which does not have a connection associated with it.

Consider the following diagram. In this diagram, `alice0` and `alice1` represent two replicas of ACA-Py working collectively to represent an Alice agent. `bob` represents the remote agent.

![offer-cred-cache-conn-failure](https://github.com/hyperledger/aries-cloudagent-python/assets/22032832/a9c36980-04ed-4704-9b35-2c49cd20b15c)

If the loadbalancing of the replicas happens to cause the above handling of messages by the different replicas, we see the error pasted above on `bob`.

This can also happen with a slightly different sequence of messages, as shown in this diagram:

![issue-cred-cache-conn-failure](https://github.com/hyperledger/aries-cloudagent-python/assets/22032832/5ed1b63e-2273-4484-b706-2da01954e9ea)

In this case, this results in the following error on `bob`:

```
Traceback (most recent call last):
  File "/usr/lib/python3.9/asyncio/tasks.py", line 256, in __step
    result = coro.send(None)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/core/dispatcher.py", line 264, in handle_message
    await handler(context, responder)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/protocols/issue_credential/v2_0/handlers/cred_issue_handler.py", line 49, in handle
    raise HandlerException(
aries_cloudagent.messaging.base_handler.HandlerException: No connection or associated connectionless exchange found for credential
```

### The Solution

The solution implemented by this PR is to only cache connection targets on completion of a DID Exchange or connection; or, in other words, only cache connection targets for connections that have reached a `completed` state. Given that the connection target is intentionally changed in the process of these protocols (you could even say that's kind of the whole point of the protocol), I believe there is little benefit to caching the initial connection target anyways. This notion is supported by these lines:

https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/connections/models/conn_record.py#L503-L513

```
    async def post_save(self, session: ProfileSession, *args, **kwargs):
        """Perform post-save actions.

        Args:
            session: The active profile session
        """
        await super().post_save(session, *args, **kwargs)

        # clear cache key set by connection manager
        cache_key = f"connection_target::{self.connection_id}"
        await self.clear_cached_key(session, cache_key)
```

After every save on the connection record (which will occur at basically every step of the did exchange or connection protocols), we're clearing the cache of the target.

Given that the cache is being cleared, causing the connection target info to be recalled from the wallet record, I believe the changes made in this PR should not impact performance, though I have not tested this.

I get the feeling this change could improve other scenarios we've seen previously that motivated the creation of the redis cache plugin but I have not tested these other scenarios.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 16:29:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2239" class=".btn">#2239</a>
            </td>
            <td>
                <b>
                    Improve faber agent with ngrok selection and invitation_url output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update NGROK_ENDPOINT to select the tunnel with the specified AGENT_PORT
- Add output of invitation_url using log_msg function
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 08:12:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2238" class=".btn">#2238</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.30.0 to 2.31.0 in /demo/playground/scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [requests](https://github.com/psf/requests) from 2.30.0 to 2.31.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.31.0</h2>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<ul>
<li>
<p>Versions of Requests between v2.3.0 and v2.30.0 are vulnerable to potential
forwarding of <code>Proxy-Authorization</code> headers to destination servers when
following HTTPS redirects.</p>
<p>When proxies are defined with user info (<a href="https://user:pass@proxy:8080">https://user:pass@proxy:8080</a>), Requests
will construct a <code>Proxy-Authorization</code> header that is attached to the request to
authenticate with the proxy.</p>
<p>In cases where Requests receives a redirect response, it previously reattached
the <code>Proxy-Authorization</code> header incorrectly, resulting in the value being
sent through the tunneled connection to the destination server. Users who rely on
defining their proxy credentials in the URL are <em>strongly</em> encouraged to upgrade
to Requests 2.31.0+ to prevent unintentional leakage and rotate their proxy
credentials once the change has been fully deployed.</p>
<p>Users who do not use a proxy or do not supply their proxy credentials through
the user information portion of their proxy URL are not subject to this
vulnerability.</p>
<p>Full details can be read in our <a href="https://github.com/psf/requests/security/advisories/GHSA-j8r2-6x86-q33q">Github Security Advisory</a>
and <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-32681">CVE-2023-32681</a>.</p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/147c8511ddbfa5e8f71bbf5c18ede0c4ceb3bba4"><code>147c851</code></a> v2.31.0</li>
<li><a href="https://github.com/psf/requests/commit/74ea7cf7a6a27a4eeb2ae24e162bcc942a6706d5"><code>74ea7cf</code></a> Merge pull request from GHSA-j8r2-6x86-q33q</li>
<li><a href="https://github.com/psf/requests/commit/302225334678490ec66b3614a9dddb8a02c5f4fe"><code>3022253</code></a> test on pypy 3.8 and pypy 3.9 on windows and macos (<a href="https://redirect.github.com/psf/requests/issues/6424">#6424</a>)</li>
<li><a href="https://github.com/psf/requests/commit/b639e66c816514e40604d46f0088fbceec1a5149"><code>b639e66</code></a> test on py3.12 (<a href="https://redirect.github.com/psf/requests/issues/6448">#6448</a>)</li>
<li><a href="https://github.com/psf/requests/commit/d3d504436ef0c2ac7ec8af13738b04dcc8c694be"><code>d3d5044</code></a> Fixed a small typo (<a href="https://redirect.github.com/psf/requests/issues/6452">#6452</a>)</li>
<li>See full diff in <a href="https://github.com/psf/requests/compare/v2.30.0...v2.31.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.30.0&new-version=2.31.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 07:14:40 +0000 UTC
    </div>
</div>

