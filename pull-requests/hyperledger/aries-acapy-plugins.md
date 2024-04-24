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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aiohttp from 3.9.2 to 3.9.4 in /oid4vci/integration/afj_runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.9.2 to 3.9.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.4</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8089">#8089</a>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8104">#8104</a>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8163">#8163</a>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7741">#7741</a>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
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
<h1>3.9.4 (2024-04-11)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8089</code>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8104</code>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8163</code>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7741</code>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b3397c7ac44fc80206d28f1dd0d1f3b10c4ec572"><code>b3397c7</code></a> Release v3.9.4 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8201">#8201</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a7e240a9f625a0b9559bdf5f0049c71565352400"><code>a7e240a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8320">#8320</a>/9ba9a4e5 backport][3.9] Fix Python parser to mark responses without...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/28335525d1eac015a7e7584137678cbb6ff19397"><code>2833552</code></a> Escape filenames and paths in HTML when generating index pages (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8317">#8317</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8319">#8319</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ed43040613988fc4666109aca82a5180ff165df5"><code>ed43040</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8309">#8309</a>/c29945a1 backport][3.9] Improve reliability of run_app test (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8315">#8315</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ec2be0500e2674eea019c0966a7a905e9b3d6608"><code>ec2be05</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8299">#8299</a>/28d026eb backport][3.9] Create marker for internal tests (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8307">#8307</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/292d961f4ee2829a1b13fad92444a4fd693fbc87"><code>292d961</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8304">#8304</a>/88c80c14 backport][3.9] Check for backports in CI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8305">#8305</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cebe526b9c34dc3a3da9140409db63014bc4cf19"><code>cebe526</code></a> Fix handling of multipart/form-data (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8280">#8280</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8302">#8302</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/270ae9cf6a9e6159b5e29a950deb6ff7600aebc5"><code>270ae9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8297">#8297</a>/d15f07cf backport][3.9] Upgrade to llhttp 9.2.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8292">#8292</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8298">#8298</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bb231059b14277c34a8a0331e51406d5abe4f424"><code>bb23105</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8283">#8283</a>/54e13b0a backport][3.9] Fix blocking I/O in the event loop while pr...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3f79241bcbc02c9850348fc04c064fcbc980e8f0"><code>3f79241</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8286">#8286</a>/28f1fd88 backport][3.9] docs: remove repetitive word in comment (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8">#8</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.2...v3.9.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.9.2&new-version=3.9.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-18 15:55:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aiohttp from 3.9.2 to 3.9.4 in /oid4vci/integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.9.2 to 3.9.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.4</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8089">#8089</a>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8104">#8104</a>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8163">#8163</a>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7741">#7741</a>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
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
<h1>3.9.4 (2024-04-11)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8089</code>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8104</code>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8163</code>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7741</code>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b3397c7ac44fc80206d28f1dd0d1f3b10c4ec572"><code>b3397c7</code></a> Release v3.9.4 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8201">#8201</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a7e240a9f625a0b9559bdf5f0049c71565352400"><code>a7e240a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8320">#8320</a>/9ba9a4e5 backport][3.9] Fix Python parser to mark responses without...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/28335525d1eac015a7e7584137678cbb6ff19397"><code>2833552</code></a> Escape filenames and paths in HTML when generating index pages (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8317">#8317</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8319">#8319</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ed43040613988fc4666109aca82a5180ff165df5"><code>ed43040</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8309">#8309</a>/c29945a1 backport][3.9] Improve reliability of run_app test (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8315">#8315</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ec2be0500e2674eea019c0966a7a905e9b3d6608"><code>ec2be05</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8299">#8299</a>/28d026eb backport][3.9] Create marker for internal tests (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8307">#8307</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/292d961f4ee2829a1b13fad92444a4fd693fbc87"><code>292d961</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8304">#8304</a>/88c80c14 backport][3.9] Check for backports in CI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8305">#8305</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cebe526b9c34dc3a3da9140409db63014bc4cf19"><code>cebe526</code></a> Fix handling of multipart/form-data (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8280">#8280</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8302">#8302</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/270ae9cf6a9e6159b5e29a950deb6ff7600aebc5"><code>270ae9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8297">#8297</a>/d15f07cf backport][3.9] Upgrade to llhttp 9.2.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8292">#8292</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8298">#8298</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bb231059b14277c34a8a0331e51406d5abe4f424"><code>bb23105</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8283">#8283</a>/54e13b0a backport][3.9] Fix blocking I/O in the event loop while pr...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3f79241bcbc02c9850348fc04c064fcbc980e8f0"><code>3f79241</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8286">#8286</a>/28f1fd88 backport][3.9] docs: remove repetitive word in comment (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8">#8</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.2...v3.9.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.9.2&new-version=3.9.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-18 15:54:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aiohttp from 3.9.2 to 3.9.4 in /redis_events/docker/services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.9.2 to 3.9.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.9.4</h2>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8089">#8089</a>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8104">#8104</a>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8163">#8163</a>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7741">#7741</a>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
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
<h1>3.9.4 (2024-04-11)</h1>
<h2>Bug fixes</h2>
<ul>
<li>
<p>The asynchronous internals now set the underlying causes
when assigning exceptions to the future objects
-- by :user:<code>webknjaz</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8089</code>.</p>
</li>
<li>
<p>Treated values of <code>Accept-Encoding</code> header as case-insensitive when checking
for gzip files -- by :user:<code>steverep</code>.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8104</code>.</p>
</li>
<li>
<p>Improved the DNS resolution performance on cache hit -- by :user:<code>bdraco</code>.</p>
<p>This is achieved by avoiding an :mod:<code>asyncio</code> task creation in this case.</p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>8163</code>.</p>
</li>
<li>
<p>Changed the type annotations to allow <code>dict</code> on :meth:<code>aiohttp.MultipartWriter.append</code>,
:meth:<code>aiohttp.MultipartWriter.append_json</code> and
:meth:<code>aiohttp.MultipartWriter.append_form</code> -- by :user:<code>cakemanny</code></p>
<p><em>Related issues and pull requests on GitHub:</em>
:issue:<code>7741</code>.</p>
</li>
<li>
<p>Ensure websocket transport is closed when client does not close it
-- by :user:<code>bdraco</code>.</p>
<p>The transport could remain open if the client did not close it. This
change ensures the transport is closed when the client does not close
it.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b3397c7ac44fc80206d28f1dd0d1f3b10c4ec572"><code>b3397c7</code></a> Release v3.9.4 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8201">#8201</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a7e240a9f625a0b9559bdf5f0049c71565352400"><code>a7e240a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8320">#8320</a>/9ba9a4e5 backport][3.9] Fix Python parser to mark responses without...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/28335525d1eac015a7e7584137678cbb6ff19397"><code>2833552</code></a> Escape filenames and paths in HTML when generating index pages (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8317">#8317</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8319">#8319</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ed43040613988fc4666109aca82a5180ff165df5"><code>ed43040</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8309">#8309</a>/c29945a1 backport][3.9] Improve reliability of run_app test (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8315">#8315</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/ec2be0500e2674eea019c0966a7a905e9b3d6608"><code>ec2be05</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8299">#8299</a>/28d026eb backport][3.9] Create marker for internal tests (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8307">#8307</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/292d961f4ee2829a1b13fad92444a4fd693fbc87"><code>292d961</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8304">#8304</a>/88c80c14 backport][3.9] Check for backports in CI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8305">#8305</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/cebe526b9c34dc3a3da9140409db63014bc4cf19"><code>cebe526</code></a> Fix handling of multipart/form-data (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8280">#8280</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8302">#8302</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/270ae9cf6a9e6159b5e29a950deb6ff7600aebc5"><code>270ae9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8297">#8297</a>/d15f07cf backport][3.9] Upgrade to llhttp 9.2.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8292">#8292</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8298">#8298</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bb231059b14277c34a8a0331e51406d5abe4f424"><code>bb23105</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8283">#8283</a>/54e13b0a backport][3.9] Fix blocking I/O in the event loop while pr...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3f79241bcbc02c9850348fc04c064fcbc980e8f0"><code>3f79241</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/8286">#8286</a>/28f1fd88 backport][3.9] docs: remove repetitive word in comment (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/8">#8</a>...</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.9.2...v3.9.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.9.2&new-version=3.9.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-18 15:53:30 +0000 UTC
    </div>
</div>

