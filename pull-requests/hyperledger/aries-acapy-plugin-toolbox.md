---
layout: default
title: aries-acapy-plugin-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugin-toolbox
---

# aries-acapy-plugin-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugin-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aiohttp from 3.8.1 to 3.8.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.8.1 to 3.8.5.
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
<h2>3.8.4</h2>
<h2>Bugfixes</h2>
<ul>
<li>Fixed incorrectly overwriting cookies with the same name and domain, but different path.
(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/6638">#6638</a>)</li>
<li>Fixed <code>ConnectionResetError</code> not being raised after client disconnection in SSL environments.
(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7180">#7180</a>)</li>
</ul>
<hr />
<h2>3.8.3</h2>
<p>.. attention::</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h1>3.8.4 (2023-02-12)</h1>
<h2>Bugfixes</h2>
<ul>
<li>Fixed incorrectly overwriting cookies with the same name and domain, but different path.
<code>[#6638](https://github.com/aio-libs/aiohttp/issues/6638) &lt;https://github.com/aio-libs/aiohttp/issues/6638&gt;</code>_</li>
<li>Fixed <code>ConnectionResetError</code> not being raised after client disconnection in SSL environments.
<code>[#7180](https://github.com/aio-libs/aiohttp/issues/7180) &lt;https://github.com/aio-libs/aiohttp/issues/7180&gt;</code>_</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.8.1...v3.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.8.1&new-version=3.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugin-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 15:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aiohttp from 3.8.1 to 3.8.5 in /int
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.8.1 to 3.8.5.
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
<h2>3.8.4</h2>
<h2>Bugfixes</h2>
<ul>
<li>Fixed incorrectly overwriting cookies with the same name and domain, but different path.
(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/6638">#6638</a>)</li>
<li>Fixed <code>ConnectionResetError</code> not being raised after client disconnection in SSL environments.
(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7180">#7180</a>)</li>
</ul>
<hr />
<h2>3.8.3</h2>
<p>.. attention::</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<h1>3.8.4 (2023-02-12)</h1>
<h2>Bugfixes</h2>
<ul>
<li>Fixed incorrectly overwriting cookies with the same name and domain, but different path.
<code>[#6638](https://github.com/aio-libs/aiohttp/issues/6638) &lt;https://github.com/aio-libs/aiohttp/issues/6638&gt;</code>_</li>
<li>Fixed <code>ConnectionResetError</code> not being raised after client disconnection in SSL environments.
<code>[#7180](https://github.com/aio-libs/aiohttp/issues/7180) &lt;https://github.com/aio-libs/aiohttp/issues/7180&gt;</code>_</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.8.1...v3.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.8.1&new-version=3.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugin-toolbox/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 15:30:53 +0000 UTC
    </div>
</div>

