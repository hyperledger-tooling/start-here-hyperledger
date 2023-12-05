---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Update ACA-Py dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves: #28 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 16:09:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Return redis_events tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bring back the redis_events integration tests that use additional plugin after repairing the build backend config line that was missing.

Also: changed the integration image names so faber using the integration dockerfile with the additional plugin is different from alice using the normal dockerfile in the docker directory.
Also: removed the `edit` condition for the PR workflow. It's not needed. 
Also: Had to add additional `$` character on the docker compose startup command on my linux machine. Not sure why? The workflow machine works with or without it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-02 16:55:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    OpenID4VCI Plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a plugin implementing the OpenID4VCI protocol (Issuance only -- future work will address OpenID4VP and I'm not sure if that should be in this plugin or a separate one). See the README for details on the implementation.

A couple of things to call out:

- This Plugin Implements Draft 11 of OpenID4VCI (https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0-11.html).
- We have been testing against the Sphereon Wallet. Kudos to the Sphereon team for their work on that!
- To interoperate with Sphereon, we needed to add support for `did:jwk` and verifying `ES256K` signatures. This implementation is within this plugin right now (as a resolver and a helper method). We plan to contribute this to ACA-Py Core.
- We plan to have automated tests against AFJ's OpenID4VCI package as soon as PR https://github.com/openwallet-foundation/agent-framework-javascript/pull/1639 is merged and released.
- Not implemented (yet):
  - `ldp_vc`, `sd_jwt_vc`
  - Authorization Code Flow
  - Only signature suite supported by ACA-Py for jwt-vc right now is `EdDSA`
  - GET /.well-known/openid-configuration
  - GET /.well-known/oauth-authorization-server
  - Batch Credential Issuance
  - We're limited to DID Methods that ACA-Py supports for issuance (more can be added by Plugin, e.g. DID Web); `did:sov`, `did:key`
  - Multitenancy Support; we need to figure out the right way to identify a sub-wallet from OpenID4VCI endpoints.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 21:42:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Repo manager fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I made a mistake with the repo manager script deleting the last line. Should have noticed it. The line was `build-backend = "poetry.core.masonry.api` The integration test in redis_events that uses basic _message storage then failed after main was updated. 

When I was fixing it I noticed that there is another problem with kafka_events and redis_events having the some of the same container names and not downing gracefully. I added a `docker compose down --remove-orphans` command to make sure the tests are being isolated.

I had to comment out the basic_message install and test cases in redis_events. I should be able to bring them back immediately after the fix is merged to main.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 19:29:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2023.5.7 to 2023.7.22 in /kafka_events/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [certifi](https://github.com/certifi/python-certifi) from 2023.5.7 to 2023.7.22.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/8fb96ed81f71e7097ed11bc4d9b19afd7ea5c909"><code>8fb96ed</code></a> 2023.07.22</li>
<li><a href="https://github.com/certifi/python-certifi/commit/afe77220e0eaa722593fc5d294213ff5275d1b40"><code>afe7722</code></a> Bump actions/setup-python from 4.6.1 to 4.7.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/230">#230</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2038739ad56abec7aaddfa90ad2ce6b3ed7f5c7b"><code>2038739</code></a> Bump dessant/lock-threads from 3.0.0 to 4.0.1 (<a href="https://redirect.github.com/certifi/python-certifi/issues/229">#229</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/44df761f4c09d19f32b3cc09208a739043a5e25b"><code>44df761</code></a> Hash pin Actions and enable dependabot (<a href="https://redirect.github.com/certifi/python-certifi/issues/228">#228</a>)</li>
<li>See full diff in <a href="https://github.com/certifi/python-certifi/compare/2023.05.07...2023.07.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2023.5.7&new-version=2023.7.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 16:30:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    chore: add dco remediation configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To help get #38 merged in, this configuration enables allowing 3rd party remediation commits.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 14:56:26 +0000 UTC
    </div>
</div>

