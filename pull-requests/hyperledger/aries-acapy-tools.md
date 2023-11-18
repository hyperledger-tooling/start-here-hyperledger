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
                PR <a href="https://github.com/hyperledger/aries-acapy-tools/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    build(deps-dev): Bump aiohttp from 3.8.5 to 3.8.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.8.5 to 3.8.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.8.6</h2>
<h2>Security bugfixes</h2>
<ul>
<li>
<p>Upgraded the vendored copy of llhttp_ to v9.1.3 -- by :user:<code>Dreamsorcerer</code></p>
<p>Thanks to :user:<code>kenballus</code> for reporting this, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-pjjw-qhg8-p2p9">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-pjjw-qhg8-p2p9</a>.</p>
<p>.. _llhttp: <a href="https://llhttp.org">https://llhttp.org</a></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7647">#7647</a>)</p>
</li>
<li>
<p>Updated Python parser to comply with RFCs 9110/9112 -- by :user:<code>Dreamorcerer</code></p>
<p>Thanks to :user:<code>kenballus</code> for reporting this, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-gfw2-4jvh-wgfg">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-gfw2-4jvh-wgfg</a>.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7663">#7663</a>)</p>
</li>
</ul>
<h2>Deprecation</h2>
<ul>
<li>
<p>Added <code>fallback_charset_resolver</code> parameter in <code>ClientSession</code> to allow a user-supplied
character set detection function.</p>
<p>Character set detection will no longer be included in 3.9 as a default. If this feature is needed,
please use <code>fallback_charset_resolver &lt;https://docs.aiohttp.org/en/stable/client_advanced.html#character-set-detection&gt;</code>_.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7561">#7561</a>)</p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li>
<p>Enabled lenient response parsing for more flexible parsing in the client
(this should resolve some regressions when dealing with badly formatted HTTP responses). -- by :user:<code>Dreamsorcerer</code></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7490">#7490</a>)</p>
</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>
<p>Fixed <code>PermissionError</code> when <code>.netrc</code> is unreadable due to permissions.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7237">#7237</a>)</p>
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
<h1>3.8.6 (2023-10-07)</h1>
<h2>Security bugfixes</h2>
<ul>
<li>
<p>Upgraded the vendored copy of llhttp_ to v9.1.3 -- by :user:<code>Dreamsorcerer</code></p>
<p>Thanks to :user:<code>kenballus</code> for reporting this, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-pjjw-qhg8-p2p9">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-pjjw-qhg8-p2p9</a>.</p>
<p>.. _llhttp: <a href="https://llhttp.org">https://llhttp.org</a></p>
<p><code>[#7647](https://github.com/aio-libs/aiohttp/issues/7647) &lt;https://github.com/aio-libs/aiohttp/issues/7647&gt;</code>_</p>
</li>
<li>
<p>Updated Python parser to comply with RFCs 9110/9112 -- by :user:<code>Dreamorcerer</code></p>
<p>Thanks to :user:<code>kenballus</code> for reporting this, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-gfw2-4jvh-wgfg">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-gfw2-4jvh-wgfg</a>.</p>
<p><code>[#7663](https://github.com/aio-libs/aiohttp/issues/7663) &lt;https://github.com/aio-libs/aiohttp/issues/7663&gt;</code>_</p>
</li>
</ul>
<h2>Deprecation</h2>
<ul>
<li>
<p>Added <code>fallback_charset_resolver</code> parameter in <code>ClientSession</code> to allow a user-supplied
character set detection function.</p>
<p>Character set detection will no longer be included in 3.9 as a default. If this feature is needed,
please use <code>fallback_charset_resolver &lt;https://docs.aiohttp.org/en/stable/client_advanced.html#character-set-detection&gt;</code>_.</p>
<p><code>[#7561](https://github.com/aio-libs/aiohttp/issues/7561) &lt;https://github.com/aio-libs/aiohttp/issues/7561&gt;</code>_</p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li>
<p>Enabled lenient response parsing for more flexible parsing in the client
(this should resolve some regressions when dealing with badly formatted HTTP responses). -- by :user:<code>Dreamsorcerer</code></p>
<p><code>[#7490](https://github.com/aio-libs/aiohttp/issues/7490) &lt;https://github.com/aio-libs/aiohttp/issues/7490&gt;</code>_</p>
</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>Fixed <code>PermissionError</code> when <code>.netrc</code> is unreadable due to permissions.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/996de2629ef6b4c2934a7c04dfd49d0950d4c43b"><code>996de26</code></a> Release v3.8.6 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7668">#7668</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/8c128d4f042ca36ebdc55ecdd76099b7722331ba"><code>8c128d4</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7651">#7651</a>/45f98b7d backport][3.8] Fix BadStatusLine message (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7666">#7666</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/89b7df157886ff390cdcdc44ecf3c277045838b1"><code>89b7df1</code></a> Allow lax response parsing on Py parser (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7663">#7663</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7664">#7664</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/d5c12ba890557a575c313bb3017910d7616fce3d"><code>d5c12ba</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7661">#7661</a>/85713a48 backport][3.8] Update Python parser for RFCs 9110/9112 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7">#7</a>...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/8a3977acac632d1f02aa7e047da51e27a717d724"><code>8a3977a</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7272">#7272</a>/b2a7983a backport][3.8] Fix Read The Docs config (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7650">#7650</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/bcc416e533796d04fb8124ef1e7686b1f338767a"><code>bcc416e</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7647">#7647</a>/1303350e backport][3.8] Upgrade to llhttp 9.1.3 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7648">#7648</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/b30c0cd2c96e57cc273ffe29c0313487b364f15a"><code>b30c0cd</code></a> Remove chardet/charset-normalizer. (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7589">#7589</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/5946c7436044bae14617ef06ee7c530ed72622da"><code>5946c74</code></a> CookieJar - return 'best-match' and not LIFO (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7577">#7577</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7588">#7588</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/8c4ec62f5ba514479ef1c2e74741bc7fa33be3f4"><code>8c4ec62</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7518">#7518</a>/8bd42e74 backport][3.8] Fix GunicornWebWorker max_requests_jitter n...</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/a0d234df392bd5cd67d378d31c9531c5ac87c07f"><code>a0d234d</code></a> Use lenient headers for response parser (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7490">#7490</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7492">#7492</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.8.5...v3.8.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.8.5&new-version=3.8.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-14 23:55:58 +0000 UTC
    </div>
</div>

