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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    Bump aiohttp from 3.8.6 to 3.9.0 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.8.6 to 3.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.0</h2>
<h2>Features</h2>
<ul>
<li>
<p>Introduced <code>AppKey</code> for static typing support of <code>Application</code> storage.
See <a href="https://docs.aiohttp.org/en/stable/web_advanced.html#application-s-config">https://docs.aiohttp.org/en/stable/web_advanced.html#application-s-config</a></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/5864">#5864</a>)</p>
</li>
<li>
<p>Added a graceful shutdown period which allows pending tasks to complete before the application's cleanup is called.
The period can be adjusted with the <code>shutdown_timeout</code> parameter. -- by :user:<code>Dreamsorcerer</code>.
See <a href="https://docs.aiohttp.org/en/latest/web_advanced.html#graceful-shutdown">https://docs.aiohttp.org/en/latest/web_advanced.html#graceful-shutdown</a></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7188">#7188</a>)</p>
</li>
<li>
<p>Added <code>handler_cancellation &lt;https://docs.aiohttp.org/en/stable/web_advanced.html#web-handler-cancellation&gt;</code>_ parameter to cancel web handler on client disconnection. -- by :user:<code>mosquito</code>
This (optionally) reintroduces a feature removed in a previous release.
Recommended for those looking for an extra level of protection against denial-of-service attacks.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7056">#7056</a>)</p>
</li>
<li>
<p>Added support for setting response header parameters <code>max_line_size</code> and <code>max_field_size</code>.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/2304">#2304</a>)</p>
</li>
<li>
<p>Added <code>auto_decompress</code> parameter to <code>ClientSession.request</code> to override <code>ClientSession._auto_decompress</code>. -- by :user:<code>Daste745</code></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/3751">#3751</a>)</p>
</li>
<li>
<p>Changed <code>raise_for_status</code> to allow a coroutine.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/3892">#3892</a>)</p>
</li>
<li>
<p>Added client brotli compression support (optional with runtime check).</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/5219">#5219</a>)</p>
</li>
<li>
<p>Added <code>client_max_size</code> to <code>BaseRequest.clone()</code> to allow overriding the request body size. -- :user:<code>anesabml</code>.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/5704">#5704</a>)</p>
</li>
<li>
<p>Added a middleware type alias <code>aiohttp.typedefs.Middleware</code>.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/5898">#5898</a>)</p>
</li>
<li>
<p>Exported <code>HTTPMove</code> which can be used to catch any redirection request
that has a location -- :user:<code>dreamsorcerer</code>.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/6594">#6594</a>)</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/master/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.9.0 (2023-11-18)</h1>
<h2>Features</h2>
<ul>
<li>
<p>Introduced <code>AppKey</code> for static typing support of <code>Application</code> storage.
See <a href="https://docs.aiohttp.org/en/stable/web_advanced.html#application-s-config">https://docs.aiohttp.org/en/stable/web_advanced.html#application-s-config</a></p>
<p><code>[#5864](https://github.com/aio-libs/aiohttp/issues/5864) &lt;https://github.com/aio-libs/aiohttp/issues/5864&gt;</code>_</p>
</li>
<li>
<p>Added a graceful shutdown period which allows pending tasks to complete before the application's cleanup is called.
The period can be adjusted with the <code>shutdown_timeout</code> parameter. -- by :user:<code>Dreamsorcerer</code>.
See <a href="https://docs.aiohttp.org/en/latest/web_advanced.html#graceful-shutdown">https://docs.aiohttp.org/en/latest/web_advanced.html#graceful-shutdown</a></p>
<p><code>[#7188](https://github.com/aio-libs/aiohttp/issues/7188) &lt;https://github.com/aio-libs/aiohttp/issues/7188&gt;</code>_</p>
</li>
<li>
<p>Added <code>handler_cancellation &lt;https://docs.aiohttp.org/en/stable/web_advanced.html#web-handler-cancellation&gt;</code>_ parameter to cancel web handler on client disconnection. -- by :user:<code>mosquito</code>
This (optionally) reintroduces a feature removed in a previous release.
Recommended for those looking for an extra level of protection against denial-of-service attacks.</p>
<p><code>[#7056](https://github.com/aio-libs/aiohttp/issues/7056) &lt;https://github.com/aio-libs/aiohttp/issues/7056&gt;</code>_</p>
</li>
<li>
<p>Added support for setting response header parameters <code>max_line_size</code> and <code>max_field_size</code>.</p>
<p><code>[#2304](https://github.com/aio-libs/aiohttp/issues/2304) &lt;https://github.com/aio-libs/aiohttp/issues/2304&gt;</code>_</p>
</li>
<li>
<p>Added <code>auto_decompress</code> parameter to <code>ClientSession.request</code> to override <code>ClientSession._auto_decompress</code>. -- by :user:<code>Daste745</code></p>
<p><code>[#3751](https://github.com/aio-libs/aiohttp/issues/3751) &lt;https://github.com/aio-libs/aiohttp/issues/3751&gt;</code>_</p>
</li>
<li>
<p>Changed <code>raise_for_status</code> to allow a coroutine.</p>
<p><code>[#3892](https://github.com/aio-libs/aiohttp/issues/3892) &lt;https://github.com/aio-libs/aiohttp/issues/3892&gt;</code>_</p>
</li>
<li>
<p>Added client brotli compression support (optional with runtime check).</p>
<p><code>[#5219](https://github.com/aio-libs/aiohttp/issues/5219) &lt;https://github.com/aio-libs/aiohttp/issues/5219&gt;</code>_</p>
</li>
<li>
<p>Added <code>client_max_size</code> to <code>BaseRequest.clone()</code> to allow overriding the request body size. -- :user:<code>anesabml</code>.</p>
<p><code>[#5704](https://github.com/aio-libs/aiohttp/issues/5704) &lt;https://github.com/aio-libs/aiohttp/issues/5704&gt;</code>_</p>
</li>
<li>
<p>Added a middleware type alias <code>aiohttp.typedefs.Middleware</code>.</p>
<p><code>[#5898](https://github.com/aio-libs/aiohttp/issues/5898) &lt;https://github.com/aio-libs/aiohttp/issues/5898&gt;</code>_</p>
</li>
<li>
<p>Exported <code>HTTPMove</code> which can be used to catch any redirection request
that has a location -- :user:<code>dreamsorcerer</code>.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/45b2c2c5773f0ee0d35fce8ff5716c78e91d9135"><code>45b2c2c</code></a> Release v3.9.0 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7843">#7843</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/5d59d3d6ac073a7db5e5d2234e03a67da5dec48a"><code>5d59d3d</code></a> Release v3.9.0rc0 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7840">#7840</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/c806814a8aaad1661d75e6e2b8d619d6c44d331d"><code>c806814</code></a> Release v3.9.0rc0 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7838">#7838</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/e07a1bdaacfb83fda3ea8f668edacb36c6c125df"><code>e07a1bd</code></a> Use timestamp instead of datetime to achieve faster cookie expiration… (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7837">#7837</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/53476dfd4ef4fb1bb74a267714bbc39eda71b403"><code>53476df</code></a> Disallow arbitrary sequence types in version (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7835">#7835</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7836">#7836</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/9d712f2f9c06f71d48e98374938813643503bc34"><code>9d712f2</code></a> Bump mypy from 1.6.1 to 1.7.0 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7833">#7833</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/63a805e1d8360fd388b6e6443cd9bdfb139e90ea"><code>63a805e</code></a> Bump python-on-whales from 0.66.0 to 0.67.0 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7832">#7832</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cb94533dd50426809b7fcbb8bbad0ef17509de5c"><code>cb94533</code></a> Ensure writer is always reset on completion (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7815">#7815</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7826">#7826</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/c0f9017a9a34a7823e1ea9b9abb393bd6c10777b"><code>c0f9017</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7821">#7821</a>/366ba40f backport][3.9] Only check origin if insecure scheme and th...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/9d498ca1e632fe1976ea1dae0ea083b29b0cc4c0"><code>9d498ca</code></a> Bump sphinx from 7.1.1 to 7.2.6 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7606">#7606</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.8.6...v3.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.8.6&new-version=3.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-28 01:00:12 +0000 UTC
    </div>
</div>

