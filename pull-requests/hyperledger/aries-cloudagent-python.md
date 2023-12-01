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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2643" class=".btn">#2643</a>
            </td>
            <td>
                <b>
                    Initial migration of anoncreds revocation code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 19:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2642" class=".btn">#2642</a>
            </td>
            <td>
                <b>
                    Feat: DIDX Implicit Request auto-accept and Delete OOB Invitation related records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #2644
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 16:57:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2638" class=".btn">#2638</a>
            </td>
            <td>
                <b>
                    fix: update broken demo dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couldn't proceed with further local testing on my host. Probably due to differences in python versions. 

```
    self.proc = await asyncio.wait_for(future, 20, loop=loop)
                      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
TypeError: wait_for() got an unexpected keyword argument 'loop'
```

But pip install works fine now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 14:22:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2636" class=".btn">#2636</a>
            </td>
            <td>
                <b>
                    Bump cryptography from 41.0.5 to 41.0.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 41.0.5 to 41.0.6.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.6 - 2023-11-27</p>
<pre><code>
* Fixed a null-pointer-dereference and segfault that could occur when loading
  certificates from a PKCS#7 bundle.  Credit to **pkuzco** for reporting the
  issue. **CVE-2023-49083**
<p>.. _v41-0-5:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/f09c261ca10a31fe41b1262306db7f8f1da0e48a"><code>f09c261</code></a> 41.0.6 release (<a href="https://redirect.github.com/pyca/cryptography/issues/9927">#9927</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/41.0.5...41.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=41.0.5&new-version=41.0.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 00:26:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2635" class=".btn">#2635</a>
            </td>
            <td>
                <b>
                    Bump aiohttp from 3.8.6 to 3.9.0
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 00:55:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2633" class=".btn">#2633</a>
            </td>
            <td>
                <b>
                    Anoncreds rs sync up with main branch
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
        Created At 2023-11-27 18:54:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2632" class=".btn">#2632</a>
            </td>
            <td>
                <b>
                    Integrate Anoncreds rs into credential and presentation endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Incorporate the new `askar-anoncreds` wallet type into the Credential and Presentation (`V2.0` only!) endpoints.  Update demo and integration tests and add a document.

Revocation support (for anoncreds) is still outstanding, this is the next task.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-27 18:28:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2630" class=".btn">#2630</a>
            </td>
            <td>
                <b>
                    Feature Suggestion: Include a Reason When Constraints Cannot Be Applied
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When the verifier agent is unable to apply a constraint filter, it would be helpful for the Problem Report to include a reason why it failed. For example, instead of:

```
Constraint specified for input_descriptor_123 does not apply to the enclosed credential in $.verifiableCredential[0]
```

... the message could include the reason that the constraint could not be applied, with the specific path or item that did not match. For example:

```
Constraint specified for input_descriptor_123 does not apply to the enclosed credential in $.verifiableCredential[0]
Reason: Credential is not applicable for field 11111111-2222-3333-4444-56789abcdef0 with paths ['$.credentialSubject.part1.part2']
```

This indicates that the field indicated in the message was not found in the Reveal Document or the full Credential.

or

```
Constraint specified for input_descriptor_123 does not apply to the enclosed credential in $.verifiableCredential[0]
Reason: No field in constraints for part2 under parent path "$.credentialSubject.part1"
```

This indicates that the "part2" property found in the Reveal Document under "$.credentialSubject.part1" was not found in the list of fields in the constraints.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 22:22:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2629" class=".btn">#2629</a>
            </td>
            <td>
                <b>
                    Update the ReadTheDocs config in case we do another 0.10.x release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This file has not been updated for the last two releases, and as such, the ReadTheDocs deployments have not worked. Not the end of the world, but adding this file now in case we do another release, and I forget again. If we don't do another deploy -- no harm done.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 18:52:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2627" class=".btn">#2627</a>
            </td>
            <td>
                <b>
                    0.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 0.11.0 release -- including adding the CHANGELOG entries for releases 0.10.2 - 0.10.5 to the main branch CHANGELOG.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 23:06:39 +0000 UTC
    </div>
</div>

