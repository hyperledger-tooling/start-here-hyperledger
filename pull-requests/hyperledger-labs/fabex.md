---
layout: default
title: fabex
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabex
---

# fabex <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabex){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabex/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    Bump github.com/gin-gonic/gin from 1.6.3 to 1.7.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/gin-gonic/gin](https://github.com/gin-gonic/gin) from 1.6.3 to 1.7.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/gin-gonic/gin/releases">github.com/gin-gonic/gin's releases</a>.</em></p>
<blockquote>
<h2>Release v1.7.7</h2>
<h3>BUGFIXES</h3>
<ul>
<li>Fixed X-Forwarded-For unsafe handling of CVE-2020-28483 <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2844">#2844</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2862">#2862</a></li>
<li>Tree: updated the code logic for <code>latestNode</code> <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2897">#2897</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2894">#2894</a> <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2878">#2878</a></li>
<li>Tree: fixed the misplacement of adding slashes <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2847">#2847</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2843">#2843</a></li>
<li>Tree: fixed tsr with mixed static and wildcard paths <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2924">#2924</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2918">#2918</a></li>
</ul>
<h3>ENHANCEMENTS</h3>
<ul>
<li>TrustedProxies: make it backward-compatible <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2887">#2887</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2819">#2819</a></li>
<li>TrustedPlatform: provide custom options for another CDN services <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2906">#2906</a></li>
</ul>
<h3>DOCS</h3>
<ul>
<li>NoMethod: added usage annotation (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2832#issuecomment-929954463">#2832</a>)</li>
</ul>
<h2>Release v1.7.6</h2>
<p>Handle pre release v1.7.5 error, so release v1.7.6 but still use v1.7.4 codes.</p>
<h2>bump new release to fix checksum mismatch</h2>
<p>No release notes provided.</p>
<h2>v1.7.3</h2>
<h3>BUGFIXES</h3>
<ul>
<li>fix level 1 router match <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2767">#2767</a>, <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2796">#2796</a></li>
</ul>
<h2>release v1.7.2</h2>
<h3>BUGFIXES</h3>
<ul>
<li>Fix conflict between param and exact path <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2706">#2706</a>. Close issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2682">#2682</a> <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2696">#2696</a>.</li>
</ul>
<h2>v1.7.1</h2>
<h3>BUGFIXES</h3>
<ul>
<li>fix: data race with trustedCIDRs from <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2674">#2674</a>(<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2675">#2675</a>)</li>
</ul>
<h2>Release v1.7.0</h2>
<h3>BUGFIXES</h3>
<ul>
<li>fix compile error from <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2572">#2572</a> (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2600">#2600</a>)</li>
<li>fix: print headers without Authorization header on broken pipe (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2528">#2528</a>)</li>
<li>fix(tree): reassign fullpath when register new node (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2366">#2366</a>)</li>
</ul>
<h3>ENHANCEMENTS</h3>
<ul>
<li>Support params and exact routes without creating conflicts (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2663">#2663</a>)</li>
<li>chore: improve render string performance (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2365">#2365</a>)</li>
<li>Sync route tree to httprouter latest code (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2368">#2368</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/gin-gonic/gin/blob/master/CHANGELOG.md">github.com/gin-gonic/gin's changelog</a>.</em></p>
<blockquote>
<h2>Gin v1.7.7</h2>
<h3>BUGFIXES</h3>
<ul>
<li>Fixed X-Forwarded-For unsafe handling of CVE-2020-28483 <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2844">#2844</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2862">#2862</a>.</li>
<li>Tree: updated the code logic for <code>latestNode</code> <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2897">#2897</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2894">#2894</a> <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2878">#2878</a>.</li>
<li>Tree: fixed the misplacement of adding slashes <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2847">#2847</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2843">#2843</a>.</li>
<li>Tree: fixed tsr with mixed static and wildcard paths <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2924">#2924</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2918">#2918</a>.</li>
</ul>
<h3>ENHANCEMENTS</h3>
<ul>
<li>TrustedProxies: make it backward-compatible <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2887">#2887</a>, closed issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2819">#2819</a>.</li>
<li>TrustedPlatform: provide custom options for another CDN services <a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2906">#2906</a>.</li>
</ul>
<h3>DOCS</h3>
<ul>
<li>NoMethod: added usage annotation (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2832#issuecomment-929954463">#2832</a>).</li>
</ul>
<h2>Gin v1.7.6</h2>
<h3>BUGFIXES</h3>
<ul>
<li>bump new release to fix v1.7.5 release error by using v1.7.4 codes.</li>
</ul>
<h2>Gin v1.7.4</h2>
<h3>BUGFIXES</h3>
<ul>
<li>bump new release to fix checksum mismatch</li>
</ul>
<h2>Gin v1.7.3</h2>
<h3>BUGFIXES</h3>
<ul>
<li>fix level 1 router match <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2767">#2767</a>, <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2796">#2796</a></li>
</ul>
<h2>Gin v1.7.2</h2>
<h3>BUGFIXES</h3>
<ul>
<li>Fix conflict between param and exact path <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2706">#2706</a>. Close issue <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2682">#2682</a> <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2696">#2696</a>.</li>
</ul>
<h2>Gin v1.7.1</h2>
<h3>BUGFIXES</h3>
<ul>
<li>fix: data race with trustedCIDRs from <a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2674">#2674</a>(<a href="https://github-redirect.dependabot.com/gin-gonic/gin/pull/2675">#2675</a>)</li>
</ul>
<h2>Gin v1.7.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/gin-gonic/gin/commit/84d927b8ad57ed9e1cda240b41fa2eed55066103"><code>84d927b</code></a> chore(docs): Bump to v1.7.7 (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2952">#2952</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/2d3572ae5c66ebcb9f83ebc1fb0882b3201608cd"><code>2d3572a</code></a> Update version.go (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2923">#2923</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/ae6f7a30475ec4c04eb05bbff0454c2ba4c8015e"><code>ae6f7a3</code></a> fix tsr with mixed static and wildcard paths (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2924">#2924</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/bb945cfa1cb6eac02bbe308dc509bd598502c16f"><code>bb945cf</code></a> fix the misplacement of adding slashes (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2847">#2847</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/a3f087277fabe5d7498ce867d2eebec379460dcd"><code>a3f0872</code></a> Provide custom options of TrustedPlatform for another CDN services (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2906">#2906</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/b5ad462601eac5cf23095c9ecf419be164497748"><code>b5ad462</code></a> Update the code logic for latestNode in tree.go (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2897">#2897</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/3b555a560534ca3114515c4b32737ba51b10392c"><code>3b555a5</code></a> ClientIP: check every proxy for trustiness (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2844">#2844</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/fc5d6dd1135f1cc66d8923f06aadb3cfc49ec0b5"><code>fc5d6dd</code></a> Tidy: Complete TrustedProxies feature (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2887">#2887</a>)</li>
<li><a href="https://github.com/gin-gonic/gin/commit/7d2091402e990ff7ffffe8446554ab8449db1a95"><code>7d20914</code></a> Quick Fix c.ClientIP() mistakely parsing to 127.0.0.1 for who not using r.Run...</li>
<li><a href="https://github.com/gin-gonic/gin/commit/4ad9526095f7f01672d89e365f0f55c5d6cba272"><code>4ad9526</code></a> Fix grammatical and spelling errors in context.go (<a href="https://github-redirect.dependabot.com/gin-gonic/gin/issues/2883">#2883</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/gin-gonic/gin/compare/v1.6.3...v1.7.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/gin-gonic/gin&package-manager=go_modules&previous-version=1.6.3&new-version=1.7.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabex/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 21:17:26 +0000 UTC
    </div>
</div>

