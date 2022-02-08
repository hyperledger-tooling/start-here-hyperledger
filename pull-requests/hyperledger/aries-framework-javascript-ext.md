---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    chore: release @aries-framework/rest 0.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">autorelease: pending</span>
            </td>
            <td>
                :robot: I have created a release \*beep\* \*boop\*
---
## [0.8.0](https://www.github.com/hyperledger/aries-framework-javascript-ext/compare/rest-v0.7.0...rest-v0.8.0) (2022-02-06)


### Features

* **rest:** add webhooks ([#93](https://www.github.com/hyperledger/aries-framework-javascript-ext/issues/93)) ([9fc020d](https://www.github.com/hyperledger/aries-framework-javascript-ext/commit/9fc020d7db0f002894e520766987eec327a2ed69))
---


This PR was generated with [Release Please](https://github.com/googleapis/release-please). See [documentation](https://github.com/googleapis/release-please#release-please).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-06 15:19:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    build(deps): bump node-fetch from 2.2.0 to 2.6.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.2.0 to 2.6.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v2.6.7</h2>
<h1>Security patch release</h1>
<p>Recommended to upgrade, to not leak sensitive cookie and authentication header information to 3th party host while a redirect occurred</p>
<h2>What's Changed</h2>
<ul>
<li>fix: don't forward secure headers to 3th party by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1453">node-fetch/node-fetch#1453</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7">https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7</a></p>
<h2>v2.6.6</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(URL): prefer built in URL version when available and fallback to whatwg by <a href="https://github.com/jimmywarting"><code>@​jimmywarting</code></a> in <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/pull/1352">node-fetch/node-fetch#1352</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6">https://github.com/node-fetch/node-fetch/compare/v2.6.5...v2.6.6</a></p>
<h2>v2.6.2</h2>
<p>fixed main path in package.json</p>
<h2>v2.6.1</h2>
<p><strong>This is an important security release. It is strongly recommended to update as soon as possible.</strong></p>
<p>See <a href="https://github.com/node-fetch/node-fetch/blob/master/docs/CHANGELOG.md#v261">CHANGELOG</a> for details.</p>
<h2>v2.6.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.6.0/CHANGELOG.md#v260">CHANGELOG</a>.</p>
<h2>v2.5.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.5.0/CHANGELOG.md#v250">CHANGELOG</a>.</p>
<h2>v2.4.1</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.4.1/CHANGELOG.md#v241">CHANGELOG</a>.</p>
<h2>v2.4.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.4.0/CHANGELOG.md#v240">CHANGELOG</a>.</p>
<h2>v2.3.0</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.3.0/CHANGELOG.md#v230">CHANGELOG</a>.</p>
<h2>v2.2.1</h2>
<p>See <a href="https://github.com/bitinn/node-fetch/blob/v2.2.1/CHANGELOG.md#v221">CHANGELOG</a>.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1ef4b560a17e644a02a3bfdea7631ffeee578b35"><code>1ef4b56</code></a> backport of <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1453">#1453</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8fe5c4ea66b9b8187600e6d5ec9b1b6781f44009"><code>8fe5c4e</code></a> 2.x: Specify encoding as an optional peer dependency in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1310">#1310</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/f56b0c66d3dd2ef185436de1f2fd40f66bfea8f4"><code>f56b0c6</code></a> fix(URL): prefer built in URL version when available and fallback to whatwg (...</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5417aea6a3275932283a200214522e6ab53f1ea"><code>b5417ae</code></a> fix: import whatwg-url in a way compatible with ESM Node (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1303">#1303</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/18193c5922c64046b922e18faf41821290535f06"><code>18193c5</code></a> fix v2.6.3 that did not sending query params (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1301">#1301</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/ace7536c955556be742d9910566738630cc3c2a6"><code>ace7536</code></a> fix: properly encode url with unicode characters (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1291">#1291</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/152214ca2f6e2a5a17d71e4638114625d3be30c6"><code>152214c</code></a> Fix(package.json): Corrected main file path in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1274">#1274</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/b5e2e41b2b50bf2997720d6125accaf0dd68c0ab"><code>b5e2e41</code></a> update version number</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/2358a6c2563d1730a0cdaccc197c611949f6a334"><code>2358a6c</code></a> Honor the <code>size</code> option after following a redirect and revert data uri support</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8c197f8982a238b3c345c64b17bfa92e16b4f7c4"><code>8c197f8</code></a> docs: Fix typos and grammatical errors in README.md (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/686">#686</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/node-fetch/node-fetch/compare/v2.2.0...v2.6.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.2.0&new-version=2.6.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
Dependabot will merge this PR once it's up-to-date and CI passes on it, as requested by @TimoGlastra.

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript-ext/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-06 15:13:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    feat: rest webhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #63 
Signed-off-by: annelein <anneleinvanreijen@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 14:44:48 +0000 UTC
    </div>
</div>

