---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    Bump undici from 5.9.1 to 5.19.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.9.1 to 5.19.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.19.1</h2>
<h2>⚠️ Security Release ⚠️</h2>
<ul>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-r6ch-mqf9-qc9w">Regular Expression Denial of Service in Headers</a> with CVE-2023-24807</li>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-5r9g-qh6m-jxff">CRLF Injection in Nodejs ‘undici’ via host</a> with CVE-2023-23936</li>
</ul>
<p>This release is part of the Node.js security release train: <a href="https://nodejs.org/en/blog/vulnerability/february-2023-security-releases/">https://nodejs.org/en/blog/vulnerability/february-2023-security-releases/</a></p>
<h2>v5.19.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(fetch): raise AbortSignal max event listeners by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1910">nodejs/undici#1910</a></li>
<li>fix: content-disposition header parsing by <a href="https://github.com/climba03003"><code>@​climba03003</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1911">nodejs/undici#1911</a></li>
<li>fix: remove test by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1916">nodejs/undici#1916</a></li>
<li>feat: add Headers.prototype.getSetCookie by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1915">nodejs/undici#1915</a></li>
<li>fix(headers): clone getSetCookie list &amp; add getSetCookie type by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1917">nodejs/undici#1917</a></li>
<li>doc(mock): update out-of-date reply documentation by <a href="https://github.com/p9f"><code>@​p9f</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1913">nodejs/undici#1913</a></li>
<li>fix(types): add missing keepAlive params by <a href="https://github.com/SkeLLLa"><code>@​SkeLLLa</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1918">nodejs/undici#1918</a></li>
<li>Make the fetch() abort test pass locally, on Linux and Mac, Node 18/19. by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1927">nodejs/undici#1927</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/climba03003"><code>@​climba03003</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1911">nodejs/undici#1911</a></li>
<li><a href="https://github.com/p9f"><code>@​p9f</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1913">nodejs/undici#1913</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.18.0...v5.19.0">https://github.com/nodejs/undici/compare/v5.18.0...v5.19.0</a></p>
<h2>v5.18.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Add ability to set TCP keepalive by <a href="https://github.com/xconverge"><code>@​xconverge</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1904">nodejs/undici#1904</a></li>
<li>use faster timers by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1908">nodejs/undici#1908</a></li>
<li>fix: ensure header value is a string by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1899">nodejs/undici#1899</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.17.1...v5.18.0">https://github.com/nodejs/undici/compare/v5.17.1...v5.18.0</a></p>
<h2>v5.17.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: bad buffer slice (<a href="https://github.com/nodejs/undici/commit/d2be675575512794dcd41b9683b209fc15368154">https://github.com/nodejs/undici/commit/d2be675575512794dcd41b9683b209fc15368154</a>)</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.17.0...v5.17.1">https://github.com/nodejs/undici/compare/v5.17.0...v5.17.1</a></p>
<h2>v5.17.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(wpts): Blob is a global getter in &gt;=v19.x.x by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1880">nodejs/undici#1880</a></li>
<li>doc: fix anchor links dispatcher.stream by <a href="https://github.com/RafaelGSS"><code>@​RafaelGSS</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1881">nodejs/undici#1881</a></li>
<li>wpt: make runner more resilient by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1884">nodejs/undici#1884</a></li>
<li>Make test pass in v19.x by <a href="https://github.com/mcollina"><code>@​mcollina</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1879">nodejs/undici#1879</a></li>
<li>Correct the type of DispatchOptions[&quot;headers&quot;] by <a href="https://github.com/pan93412"><code>@​pan93412</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1896">nodejs/undici#1896</a></li>
<li>perf(content-type parser): faster string collector by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1894">nodejs/undici#1894</a></li>
<li>feat: expose content-type parser by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1895">nodejs/undici#1895</a></li>
<li>fix(types): Update DispatchOptions type for missing &quot;blocking&quot; by <a href="https://github.com/xconverge"><code>@​xconverge</code></a> in <a href="https://github-redirect.dependabot.com/nodejs/undici/pull/1889">nodejs/undici#1889</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/984d53bad97c98529424a7f3bef6be1d0e76d039"><code>984d53b</code></a> Bumped v5.19.1</li>
<li><a href="https://github.com/nodejs/undici/commit/6c32c0fd5b874328e5e1f635e2cc431aa21cddab"><code>6c32c0f</code></a> lint fixes</li>
<li><a href="https://github.com/nodejs/undici/commit/f2324e549943f0b0937b09fb1c0c16cc7c93abdf"><code>f2324e5</code></a> Merge pull request from GHSA-r6ch-mqf9-qc9w</li>
<li><a href="https://github.com/nodejs/undici/commit/a2eff05401358f6595138df963837c24348f2034"><code>a2eff05</code></a> Merge pull request from GHSA-5r9g-qh6m-jxff</li>
<li><a href="https://github.com/nodejs/undici/commit/f5c89e5c87c7d702996b152c4ad86302b60c4181"><code>f5c89e5</code></a> Bumped v5.19.0</li>
<li><a href="https://github.com/nodejs/undici/commit/f7c6c6a4a2aef7ee3b8207c4eeab700cb0cfc7dc"><code>f7c6c6a</code></a> Make the fetch() abort test pass locally, on Linux and Mac, Node 18 and 19 (#...</li>
<li><a href="https://github.com/nodejs/undici/commit/aebb232d22e9adafce015b985093114a95b560f0"><code>aebb232</code></a> fix(types): add missing keepAlive params (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1918">#1918</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/e155c6db5cec9bc577d548fa7c7378013631c79c"><code>e155c6d</code></a> doc(mock): update out-of-date reply documentation (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1913">#1913</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/87fa73498d6014a33989179cfaa4347dcb29600f"><code>87fa734</code></a> fix(headers): clone getSetCookie list &amp; add getSetCookie type (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1917">#1917</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ba5ef44b71eff5a86a8473850a326ff7392664d3"><code>ba5ef44</code></a> feat: add Headers.prototype.getSetCookie (<a href="https://github-redirect.dependabot.com/nodejs/undici/issues/1915">#1915</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.9.1...v5.19.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.9.1&new-version=5.19.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 23:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/665" class=".btn">#665</a>
            </td>
            <td>
                <b>
                    Bump cacheable-request and nodemon
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Removes [cacheable-request](https://github.com/jaredwray/cacheable-request). It's no longer used after updating ancestor dependency [nodemon](https://github.com/remy/nodemon). These dependencies need to be updated together.

Removes `cacheable-request`

Updates `nodemon` from 2.0.16 to 2.0.20
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/remy/nodemon/releases">nodemon's releases</a>.</em></p>
<blockquote>
<h2>v2.0.20</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.19...v2.0.20">2.0.20</a> (2022-09-16)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>remove postinstall script (<a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0">e099e91</a>)</li>
</ul>
<h2>v2.0.19</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.18...v2.0.19">2.0.19</a> (2022-07-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Replace update notifier with simplified deps (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2033">#2033</a>) (<a href="https://github.com/remy/nodemon/commit/176c4a6bed989fe94f103c905e5eee341d26794d">176c4a6</a>), closes <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1961">#1961</a> <a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2028">#2028</a></li>
</ul>
<h2>v2.0.18</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.17...v2.0.18">2.0.18</a> (2022-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>revert update-notifier forcing esm (<a href="https://github.com/remy/nodemon/commit/1b3bc8c3c839024d0de4392f56be571a4b660754">1b3bc8c</a>)</li>
</ul>
<h2>v2.0.17</h2>
<h2><a href="https://github.com/remy/nodemon/compare/v2.0.16...v2.0.17">2.0.17</a> (2022-06-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>bump update-notifier to v6.0.0 (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2029">#2029</a>) (<a href="https://github.com/remy/nodemon/commit/0144e4ff3e26ac7f8b3d1ee19fd9fd72f827780f">0144e4f</a>)</li>
<li>update packge-lock (<a href="https://github.com/remy/nodemon/commit/27e91c36819d510a3e64111957a8ce13f0e186bc">27e91c3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/remy/nodemon/commit/e099e91cb6ff9cbb7912af86d22b91cd855a1ad0"><code>e099e91</code></a> fix: remove postinstall script</li>
<li><a href="https://github.com/remy/nodemon/commit/05de353d4de1a7e1f2aa2c9bf641c3fe2d652122"><code>05de353</code></a> chore: supports</li>
<li><a href="https://github.com/remy/nodemon/commit/876d60c8a241f13376f1b32f853d48ae77ec69a4"><code>876d60c</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/188f2d3cdc960fce5d7413e1326da76bd5be780c"><code>188f2d3</code></a> chore: supporters</li>
<li><a href="https://github.com/remy/nodemon/commit/a1ad44a876df74be742c64af5640b300c302b977"><code>a1ad44a</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/8abd3fc9daff813199042c26a1e8aa5691a5ab37"><code>8abd3fc</code></a> chore: supporters update</li>
<li><a href="https://github.com/remy/nodemon/commit/30c80f8a4eee379fa2ebad95b81c42ef11670829"><code>30c80f8</code></a> chore: add unused files to .npmignore (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/2055">#2055</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/3dd38deb4a97a52608aac148200b48d844df0a66"><code>3dd38de</code></a> docs: added link on banner (<a href="https://github-redirect.dependabot.com/remy/nodemon/issues/1944">#1944</a>)</li>
<li><a href="https://github.com/remy/nodemon/commit/fb51359dde4b4ad6081f6c2690d1052fc8f5fcaf"><code>fb51359</code></a> docs: add important note about ignore rules</li>
<li><a href="https://github.com/remy/nodemon/commit/8fe7d770d06305e5e7a4aa4ab4783d4b2c5eaac8"><code>8fe7d77</code></a> chore: supporters</li>
<li>Additional commits viewable in <a href="https://github.com/remy/nodemon/compare/v2.0.16...v2.0.20">compare view</a></li>
</ul>
</details>
<br />


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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 05:16:40 +0000 UTC
    </div>
</div>

