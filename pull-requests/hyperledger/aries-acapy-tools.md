---
layout: default
title: aries-acapy-tools
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-tools
---

# aries-acapy-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump aiohttp from 3.8.4 to 3.8.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.8.4 to 3.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.8.5</h2>
<h2>Security bugfixes</h2>
<ul>
<li>
<p>Upgraded the vendored copy of llhttp_ to v8.1.1 -- by :user:<code>webknjaz</code>
and :user:<code>Dreamsorcerer</code>.</p>
<p>Thanks to :user:<code>sethmlarson</code> for reporting this and providing us with
comprehensive reproducer, workarounds and fixing details! For more
information, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w</a>.</p>
<p>.. _llhttp: <a href="https://llhttp.org">https://llhttp.org</a></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7346">#7346</a>)</p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li>
<p>Added information to C parser exceptions to show which character caused the error. -- by :user:<code>Dreamsorcerer</code></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7366">#7366</a>)</p>
</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>
<p>Fixed a transport is :data:<code>None</code> error -- by :user:<code>Dreamsorcerer</code>.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/3355">#3355</a>)</p>
</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/v3.8.5/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.8.5 (2023-07-19)</h1>
<h2>Security bugfixes</h2>
<ul>
<li>
<p>Upgraded the vendored copy of llhttp_ to v8.1.1 -- by :user:<code>webknjaz</code>
and :user:<code>Dreamsorcerer</code>.</p>
<p>Thanks to :user:<code>sethmlarson</code> for reporting this and providing us with
comprehensive reproducer, workarounds and fixing details! For more
information, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w</a>.</p>
<p>.. _llhttp: <a href="https://llhttp.org">https://llhttp.org</a></p>
<p><code>[#7346](https://github.com/aio-libs/aiohttp/issues/7346) &lt;https://github.com/aio-libs/aiohttp/issues/7346&gt;</code>_</p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li>
<p>Added information to C parser exceptions to show which character caused the error. -- by :user:<code>Dreamsorcerer</code></p>
<p><code>[#7366](https://github.com/aio-libs/aiohttp/issues/7366) &lt;https://github.com/aio-libs/aiohttp/issues/7366&gt;</code>_</p>
</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>
<p>Fixed a transport is :data:<code>None</code> error -- by :user:<code>Dreamsorcerer</code>.</p>
<p><code>[#3355](https://github.com/aio-libs/aiohttp/issues/3355) &lt;https://github.com/aio-libs/aiohttp/issues/3355&gt;</code>_</p>
</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/9c13a52c21c23dfdb49ed89418d28a5b116d0681"><code>9c13a52</code></a> Bump aiohttp to v3.8.5 a security release</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/7c02129567bc4ec59be467b70fc937c82920948c"><code>7c02129</code></a>  Bump pypa/cibuildwheel to v2.14.1</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/135a45e9d655d56e4ebad78abe84f1cb7b5c62dc"><code>135a45e</code></a> Improve error messages from C parser (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7366">#7366</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7380">#7380</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/9337fb3f2ab2b5f38d7e98a194bde6f7e3d16c40"><code>9337fb3</code></a> Fix bump llhttp to v8.1.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7367">#7367</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7377">#7377</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/f07e9b44b5cb909054a697c8dd447b30dbf8073e"><code>f07e9b4</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7373">#7373</a>/66e261a5 backport][3.8] Drop azure mention (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7374">#7374</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/01d9b70e5477cd746561b52225992d8a2ebde953"><code>01d9b70</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7370">#7370</a>/22c264ce backport][3.8] fix: Spelling error fixed (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7371">#7371</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3577b1e3719d4648fa973dbdec927f78f9df34dd"><code>3577b1e</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7359">#7359</a>/7911f1e9 backport][3.8]  Set up secretless publishing to PyPI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7360">#7360</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/8d45f9c99511cd80140d6658bd9c11002c697f1c"><code>8d45f9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7333">#7333</a>/3a54d378 backport][3.8] Fix TLS transport is <code>None</code> error (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7357">#7357</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/dd8e24e77351df9c0f029be49d3c6d7862706e79"><code>dd8e24e</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7343">#7343</a>/18057581 backport][3.8] Mention encoding in <code>yarl.URL</code> (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7355">#7355</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/40874103ebfaa1007d47c25ecc4288af873a07cf"><code>4087410</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7346">#7346</a>/346fd202 backport][3.8]  Bump vendored llhttp to v8.1.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7352">#7352</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.8.4...v3.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.8.4&new-version=3.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 13:04:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump certifi from 2022.12.7 to 2023.7.22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [certifi](https://github.com/certifi/python-certifi) from 2022.12.7 to 2023.7.22.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/8fb96ed81f71e7097ed11bc4d9b19afd7ea5c909"><code>8fb96ed</code></a> 2023.07.22</li>
<li><a href="https://github.com/certifi/python-certifi/commit/afe77220e0eaa722593fc5d294213ff5275d1b40"><code>afe7722</code></a> Bump actions/setup-python from 4.6.1 to 4.7.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/230">#230</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2038739ad56abec7aaddfa90ad2ce6b3ed7f5c7b"><code>2038739</code></a> Bump dessant/lock-threads from 3.0.0 to 4.0.1 (<a href="https://redirect.github.com/certifi/python-certifi/issues/229">#229</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/44df761f4c09d19f32b3cc09208a739043a5e25b"><code>44df761</code></a> Hash pin Actions and enable dependabot (<a href="https://redirect.github.com/certifi/python-certifi/issues/228">#228</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/8b3d7bae85bbc87c9181cc1d39548db3d31627f0"><code>8b3d7ba</code></a> 2023.05.07</li>
<li><a href="https://github.com/certifi/python-certifi/commit/53da2405b1af430f6bafa21ba45d8dd8dfc726b8"><code>53da240</code></a> ci: Add Python 3.12-dev to the testing (<a href="https://redirect.github.com/certifi/python-certifi/issues/224">#224</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2fc3b1f64d6946f1057971ee897ea828ae848d8"><code>c2fc3b1</code></a> Create a Security Policy (<a href="https://redirect.github.com/certifi/python-certifi/issues/222">#222</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c211ef482a01aff5f1bc92c4128bfa0c955f4a01"><code>c211ef4</code></a> Set up permissions to github workflows (<a href="https://redirect.github.com/certifi/python-certifi/issues/218">#218</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2087de5d0aa1d472145fc1dbdfece3fe652bbac5"><code>2087de5</code></a> Don't let deprecation warning fail CI (<a href="https://redirect.github.com/certifi/python-certifi/issues/219">#219</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e0b9fc5c8f52ac8c300da502e5760ce3d41429ec"><code>e0b9fc5</code></a> remove paragraphs about 1024-bit roots from README</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2022.12.07...2023.07.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2022.12.7&new-version=2023.7.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 13:04:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump urllib3 from 1.26.14 to 1.26.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.26.14 to 1.26.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.17</h2>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (GHSA-v845-jxx5-vc9f)</li>
</ul>
<h2>1.26.16</h2>
<ul>
<li>Fixed thread-safety issue where accessing a <code>PoolManager</code> with many distinct origins would cause connection pools to be closed while requests are in progress (<a href="https://redirect.github.com/urllib3/urllib3/issues/2954">#2954</a>)</li>
</ul>
<h2>1.26.15</h2>
<ul>
<li>Fix socket timeout value when HTTPConnection is reused (<a href="https://redirect.github.com/urllib3/urllib3/issues/2645">urllib3/urllib3#2645</a>)</li>
<li>Remove &quot;!&quot; character from the unreserved characters in IPv6 Zone ID parsing (<a href="https://redirect.github.com/urllib3/urllib3/issues/2899">urllib3/urllib3#2899</a>)</li>
<li>Fix IDNA handling of 'x80' byte (<a href="https://redirect.github.com/urllib3/urllib3/issues/2901">urllib3/urllib3#2901</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>1.26.17 (2023-10-02)</h1>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (<code>[#3139](https://github.com/urllib3/urllib3/issues/3139) &lt;https://github.com/urllib3/urllib3/pull/3139&gt;</code>_)</li>
</ul>
<h1>1.26.16 (2023-05-23)</h1>
<ul>
<li>Fixed thread-safety issue where accessing a <code>PoolManager</code> with many distinct origins
would cause connection pools to be closed while requests are in progress (<code>[#2954](https://github.com/urllib3/urllib3/issues/2954) &lt;https://github.com/urllib3/urllib3/pull/2954&gt;</code>_)</li>
</ul>
<h1>1.26.15 (2023-03-10)</h1>
<ul>
<li>Fix socket timeout value when <code>HTTPConnection</code> is reused (<code>[#2645](https://github.com/urllib3/urllib3/issues/2645) &lt;https://github.com/urllib3/urllib3/issues/2645&gt;</code>__)</li>
<li>Remove &quot;!&quot; character from the unreserved characters in IPv6 Zone ID parsing
(<code>[#2899](https://github.com/urllib3/urllib3/issues/2899) &lt;https://github.com/urllib3/urllib3/issues/2899&gt;</code>__)</li>
<li>Fix IDNA handling of '\x80' byte (<code>[#2901](https://github.com/urllib3/urllib3/issues/2901) &lt;https://github.com/urllib3/urllib3/issues/2901&gt;</code>__)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/c9016bf464751a02b7e46f8b86504f47d4238784"><code>c9016bf</code></a> Release 1.26.17</li>
<li><a href="https://github.com/urllib3/urllib3/commit/01220354d389cd05474713f8c982d05c9b17aafb"><code>0122035</code></a> Backport GHSA-v845-jxx5-vc9f (<a href="https://redirect.github.com/urllib3/urllib3/issues/3139">#3139</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/e63989f97d206e839ab9170c8a76e3e097cc60e8"><code>e63989f</code></a> Fix installing <code>brotli</code> extra on Python 2.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2e7a24d08713a0131f0b3c7197889466d645cc49"><code>2e7a24d</code></a> [1.26] Configure OS for RTD to fix building docs</li>
<li><a href="https://github.com/urllib3/urllib3/commit/57181d6ea910ac7cb2ff83345d9e5e0eb816a0d0"><code>57181d6</code></a> [1.26] Improve error message when calling urllib3.request() (<a href="https://redirect.github.com/urllib3/urllib3/issues/3058">#3058</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/3c0148048a523325819377b23fc67f8d46afc3aa"><code>3c01480</code></a> [1.26] Run coverage even with failed jobs</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d94029b7e2193ff47b627906a70e06377a09aae8"><code>d94029b</code></a> Release 1.26.16</li>
<li><a href="https://github.com/urllib3/urllib3/commit/18e92145e9cddbabdf51c98f54202aa37fd5d4c8"><code>18e9214</code></a> Use trusted publishing for PyPI</li>
<li><a href="https://github.com/urllib3/urllib3/commit/d25cf83bbae850a290fe34ed1610ae55c0558b36"><code>d25cf83</code></a> [1.26] Fix invalid test_ssl_failure_midway_through_conn</li>
<li><a href="https://github.com/urllib3/urllib3/commit/25cca389496b86ee809c21e5b641aeaa74809263"><code>25cca38</code></a> [1.26] Fix test_ssl_object_attributes</li>
<li>Additional commits viewable in <a href="https://github.com/urllib3/urllib3/compare/1.26.14...1.26.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.26.14&new-version=1.26.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-tools/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 02:52:21 +0000 UTC
    </div>
</div>

