---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3031" class=".btn">#3031</a>
            </td>
            <td>
                <b>
                    fix(fabric-test-ledger): fix INVALID_ENDORSER_TRANSACTION error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * reverts changes of commit https://github.com/hyperledger/cacti/commit/3371772c582389f6ee0c6fb66af875dd93cc94c6, which seems to be breaking the Fabric Test Ledger

closes #3009
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 17:33:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3030" class=".btn">#3030</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump vite from 5.0.8 to 5.0.12 in /packages/cacti-ledger-browser-react
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite) from 5.0.8 to 5.0.12.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/v5.0.12/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->5.0.12 (2024-01-19)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: await <code>configResolved</code> hooks of worker plugins (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15597">#15597</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15605">#15605</a>) (<a href="https://github.com/vitejs/vite/commit/ef89f80">ef89f80</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15597">#15597</a> <a href="https://redirect.github.com/vitejs/vite/issues/15605">#15605</a></li>
<li>fix: fs deny for case insensitive systems (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15653">#15653</a>) (<a href="https://github.com/vitejs/vite/commit/91641c4">91641c4</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15653">#15653</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.0.11 (2024-01-05)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: don't pretransform classic script links (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15361">#15361</a>) (<a href="https://github.com/vitejs/vite/commit/19e3c9a">19e3c9a</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15361">#15361</a></li>
<li>fix: inject <code>__vite__mapDeps</code> code before sourcemap file comment (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15483">#15483</a>) (<a href="https://github.com/vitejs/vite/commit/d2aa096">d2aa096</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15483">#15483</a></li>
<li>fix(assets): avoid splitting <code>,</code> inside base64 value of <code>srcset</code> attribute (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15422">#15422</a>) (<a href="https://github.com/vitejs/vite/commit/8de7bd2">8de7bd2</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15422">#15422</a></li>
<li>fix(html): handle offset magic-string slice error (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15435">#15435</a>) (<a href="https://github.com/vitejs/vite/commit/5ea9edb">5ea9edb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15435">#15435</a></li>
<li>chore(deps): update dependency strip-literal to v2 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15475">#15475</a>) (<a href="https://github.com/vitejs/vite/commit/49d21fe">49d21fe</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15475">#15475</a></li>
<li>chore(deps): update tj-actions/changed-files action to v41 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15476">#15476</a>) (<a href="https://github.com/vitejs/vite/commit/2a540ee">2a540ee</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15476">#15476</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.0.10 (2023-12-15)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: omit protocol does not require pre-transform (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15355">#15355</a>) (<a href="https://github.com/vitejs/vite/commit/d9ae1b2">d9ae1b2</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15355">#15355</a></li>
<li>fix(build): use base64 for inline SVG if it contains both single and double quotes (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15271">#15271</a>) (<a href="https://github.com/vitejs/vite/commit/1bbff16">1bbff16</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15271">#15271</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.0.9 (2023-12-14)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: htmlFallbackMiddleware for favicon (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15301">#15301</a>) (<a href="https://github.com/vitejs/vite/commit/c902545">c902545</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15301">#15301</a></li>
<li>fix: more stable hash calculation for depsOptimize (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15337">#15337</a>) (<a href="https://github.com/vitejs/vite/commit/2b39fe6">2b39fe6</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15337">#15337</a></li>
<li>fix(scanner): catch all external files for glob imports (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15286">#15286</a>) (<a href="https://github.com/vitejs/vite/commit/129d0d0">129d0d0</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15286">#15286</a></li>
<li>fix(server): avoid chokidar throttling on startup (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15347">#15347</a>) (<a href="https://github.com/vitejs/vite/commit/56a5740">56a5740</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15347">#15347</a></li>
<li>fix(worker): replace <code>import.meta</code> correctly for IIFE worker (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15321">#15321</a>) (<a href="https://github.com/vitejs/vite/commit/08d093c">08d093c</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15321">#15321</a></li>
<li>feat: log re-optimization reasons (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15339">#15339</a>) (<a href="https://github.com/vitejs/vite/commit/b1a6c84">b1a6c84</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15339">#15339</a></li>
<li>chore: temporary typo (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15329">#15329</a>) (<a href="https://github.com/vitejs/vite/commit/7b71854">7b71854</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15329">#15329</a></li>
<li>perf: avoid computing paths on each request (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15318">#15318</a>) (<a href="https://github.com/vitejs/vite/commit/0506812">0506812</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15318">#15318</a></li>
<li>perf: temporary hack to avoid fs checks for /<a href="https://github.com/react-refresh"><code>@​react-refresh</code></a> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15299">#15299</a>) (<a href="https://github.com/vitejs/vite/commit/b1d6211">b1d6211</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15299">#15299</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/ee81e196769c102a6b1bf30f8444ccde236e71d5"><code>ee81e19</code></a> release: v5.0.12</li>
<li><a href="https://github.com/vitejs/vite/commit/91641c4da0a011d4c5352e88fc68389d4e1289a5"><code>91641c4</code></a> fix: fs deny for case insensitive systems (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15653">#15653</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/ef89f8092f0eb1d8fd7d21256e6af8c4e64fe9b2"><code>ef89f80</code></a> fix: await <code>configResolved</code> hooks of worker plugins (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15597">#15597</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15605">#15605</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/b44c49302ffbf0c82f984f6219ed6376d1e4552a"><code>b44c493</code></a> release: v5.0.11</li>
<li><a href="https://github.com/vitejs/vite/commit/d2aa0969ee316000d3b957d7e879f001e85e369e"><code>d2aa096</code></a> fix: inject <code>__vite__mapDeps</code> code before sourcemap file comment (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15483">#15483</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/2a540eee82f9a31deff8215bdbdccfa46d494a06"><code>2a540ee</code></a> chore(deps): update tj-actions/changed-files action to v41 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15476">#15476</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/5ea9edbc9ceb991e85f893fe62d68ed028677451"><code>5ea9edb</code></a> fix(html): handle offset magic-string slice error (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15435">#15435</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/49d21fe1feaac30dee0196bd484480a8000a4363"><code>49d21fe</code></a> chore(deps): update dependency strip-literal to v2 (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15475">#15475</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/8de7bd2b68db27b83d9484cc8d4e26436615168e"><code>8de7bd2</code></a> fix(assets): avoid splitting <code>,</code> inside base64 value of <code>srcset</code> attribute (#...</li>
<li><a href="https://github.com/vitejs/vite/commit/19e3c9a8a16847486fbad8a8cd48fc771b1538bb"><code>19e3c9a</code></a> fix: don't pretransform classic script links (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15361">#15361</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vitejs/vite/commits/v5.0.12/packages/vite">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=vite&package-manager=npm_and_yarn&previous-version=5.0.8&new-version=5.0.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-24 02:28:37 +0000 UTC
    </div>
</div>

