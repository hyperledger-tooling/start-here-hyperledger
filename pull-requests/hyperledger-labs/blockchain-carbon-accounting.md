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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/622" class=".btn">#622</a>
            </td>
            <td>
                <b>
                    Bump node-fetch from 2.6.1 to 2.6.7 in /fabric/chaincode/emissionscontract/typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.6.1 to 2.6.7.
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
<li>See full diff in <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.1...v2.6.7">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~endless">endless</a>, a new releaser for node-fetch since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.6.1&new-version=2.6.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-09-12 20:36:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    documentation for carbon tracker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @brioux Pls take a look at my comments for the carbon tracker based on today's call
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 17:22:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    Bump node-fetch from 3.2.6 to 3.2.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 3.2.6 to 3.2.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/node-fetch/node-fetch/releases">node-fetch's releases</a>.</em></p>
<blockquote>
<h2>v3.2.10</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.9...v3.2.10">3.2.10</a> (2022-07-31)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>ReDoS referrer (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1611">#1611</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/28802387292baee467e042e168d92597b5bbbe3d">2880238</a>)</li>
</ul>
<h2>v3.2.9</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.8...v3.2.9">3.2.9</a> (2022-07-18)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>Headers:</strong> don't forward secure headers on protocol change (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1599">#1599</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/e87b093fd678a9ea39c5b17b2a1bdfc4691eedc7">e87b093</a>)</li>
</ul>
<h2>v3.2.8</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.7...v3.2.8">3.2.8</a> (2022-07-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>possibly flaky test (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1523">#1523</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/11b703361134340a8361f591d6e3a0bcf6a261fa">11b7033</a>)</li>
</ul>
<h2>v3.2.7</h2>
<h2><a href="https://github.com/node-fetch/node-fetch/compare/v3.2.6...v3.2.7">3.2.7</a> (2022-07-11)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>always warn Request.data (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1550">#1550</a>) (<a href="https://github.com/node-fetch/node-fetch/commit/4f43c9ed63da98f4b5167f0a8e447cd0f0133cd3">4f43c9e</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/28802387292baee467e042e168d92597b5bbbe3d"><code>2880238</code></a> fix: ReDoS referrer (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1611">#1611</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/e87b093fd678a9ea39c5b17b2a1bdfc4691eedc7"><code>e87b093</code></a> fix(Headers): don't forward secure headers on protocol change (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1599">#1599</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/bcfb71c7d10da252280d13818daab6925e12c368"><code>bcfb71c</code></a> chore: remove triple-slash directives from typings (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1285">#1285</a>) (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1287">#1287</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/95165d5480ea0552858679a96c7f4ef001412c1b"><code>95165d5</code></a> fix spelling (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1602">#1602</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/11b703361134340a8361f591d6e3a0bcf6a261fa"><code>11b7033</code></a> fix: possibly flaky test (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1523">#1523</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/4f43c9ed63da98f4b5167f0a8e447cd0f0133cd3"><code>4f43c9e</code></a> fix: always warn Request.data (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1550">#1550</a>)</li>
<li>See full diff in <a href="https://github.com/node-fetch/node-fetch/compare/v3.2.6...v3.2.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=3.2.6&new-version=3.2.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-09-12 17:03:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    get code up to date
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
        Created At 2022-09-12 16:59:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    Add new README.md to lib folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR adds a README.md to the lib folder. The actual link to it in the main README.md is broken, since no nested README exists. I'm not deep into the listed components yet, if someone can provide a meaningful description.

Signed-off-by: Karl Seidenfad <12004185+KSilkThread@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 10:48:27 +0000 UTC
    </div>
</div>

