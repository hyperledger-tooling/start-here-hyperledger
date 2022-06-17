---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2083" class=".btn">#2083</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump electron from 13.6.6 to 15.5.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [electron](https://github.com/electron/electron) from 13.6.6 to 15.5.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/electron/electron/releases">electron's releases</a>.</em></p>
<blockquote>
<h2>electron v15.5.5</h2>
<h1>Release Notes for v15.5.5</h1>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2022-1482. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34040">#34040</a></li>
<li>Backported fix for CVE-2022-1483. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34009">#34009</a></li>
<li>Backported fix for CVE-2022-1497. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34075">#34075</a></li>
</ul>
<h2>electron v15.5.4</h2>
<h1>Release Notes for v15.5.4</h1>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2022-1138. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33682">#33682</a></li>
<li>Backported fix for CVE-2022-1478. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34045">#34045</a></li>
<li>Backported fix for CVE-2022-1479. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34037">#34037</a></li>
<li>Backported fix for CVE-2022-1480. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34019">#34019</a></li>
<li>Backported fix for CVE-2022-1492. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34051">#34051</a></li>
</ul>
<h2>electron v15.5.3</h2>
<h1>Release Notes for v15.5.3</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed a network service crash that could occur when using setCertificateVerifyProc. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33256">#33256</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/33255">16</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33254">17</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33253">18</a>)<!-- raw HTML omitted --></li>
<li><code>shell.openExternal()</code> now reports more detailed errors on Windows. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33656">#33656</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/33657">16</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33658">17</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33705">18</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33660">19</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2022-1134. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33763">#33763</a></li>
<li>Backported fix for CVE-2022-1305. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33860">#33860</a></li>
<li>Backported fix for CVE-2022-1310. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33831">#33831</a></li>
<li>Backported fix for CVE-2022-1314. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33884">#33884</a></li>
<li>Backported fix for CVE-2022-1364. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33836">#33836</a></li>
<li>Backported fix for chromium:1286816. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33679">#33679</a></li>
<li>Backported fix for chromium:1291482. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33676">#33676</a></li>
<li>Backported fix for chromium:1310761. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33856">#33856</a></li>
<li>Security: backported fix for CVE-2022-0116 and CVE-2022-1306. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33852">#33852</a></li>
<li>Security: backported fix for CVE-2022-23308. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33670">#33670</a></li>
<li>Security: backported fix for chromium:1280743. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33715">#33715</a></li>
<li>Security: backported fix for chromium:1280852. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33673">#33673</a></li>
</ul>
<h2>electron v15.5.2</h2>
<h1>Release Notes for v15.5.2</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed behavior of BrowserWindow.maximize on macOS for not shown windows. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33523">#33523</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/33535">16</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33537">18</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/electron/electron/commit/f98885312827f3f111cfac80d71dc9a2c2d2cbc9"><code>f988853</code></a> Bump v15.5.5</li>
<li><a href="https://github.com/electron/electron/commit/8bc25e8a9de07496db6b884b228ca12d0e161f07"><code>8bc25e8</code></a> build: change upload-to-s3 vars to upload-to-storage (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34142">#34142</a>)</li>
<li><a href="https://github.com/electron/electron/commit/a8f8b507aa01c794c698f72be7cc9d0f9bb9fa5b"><code>a8f8b50</code></a> build: use azure function to hash assets instead of lambda (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34119">#34119</a>)</li>
<li><a href="https://github.com/electron/electron/commit/eb320cbbf9f887ff2ecf3c76ef8b1eff7143e49f"><code>eb320cb</code></a> build: stop uploading assets to S3 (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34112">#34112</a>)</li>
<li><a href="https://github.com/electron/electron/commit/37eab5c66e609f9d98203c58feb740d23265ea2e"><code>37eab5c</code></a> chore: cherry-pick 5be8e065f43e from chromium (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34040">#34040</a>)</li>
<li><a href="https://github.com/electron/electron/commit/fc912026e2c383c24949e4bb381eb7a07121a657"><code>fc91202</code></a> chore: cherry-pick 5361d836ae from chromium (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34009">#34009</a>)</li>
<li><a href="https://github.com/electron/electron/commit/6aa0609a9707a81611b6dceb2dbd9d779c83a040"><code>6aa0609</code></a> chore: cherry-pick 6b66a45021 from chromium (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34075">#34075</a>)</li>
<li><a href="https://github.com/electron/electron/commit/620d615fe026d654178be0a462dab3580429f55a"><code>620d615</code></a> test: fix nativeModulesEnabled in spec/webview-spec.js (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34063">#34063</a>)</li>
<li><a href="https://github.com/electron/electron/commit/ec7baba40166e9f11046cff31de180e4f652ec23"><code>ec7baba</code></a> Bump v15.5.4</li>
<li><a href="https://github.com/electron/electron/commit/f8ba4d6012c2c6a853c0b9b31e2a3816ac8b3c0c"><code>f8ba4d6</code></a> chore: cherry-pick d27d9d059b51 from angle (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34045">#34045</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/electron/electron/compare/v13.6.6...v15.5.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=electron&package-manager=npm_and_yarn&previous-version=13.6.6&new-version=15.5.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 01:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2082" class=".btn">#2082</a>
            </td>
            <td>
                <b>
                    build(tools): software bill of materials generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a script to generate all SBoMs.
The short hand to call the script is by running
$ yarn generate-sbom
and then it saves all the different .spdx
files under ./dist/sbom/*
where the file names are derived from
the relative path of the directory of the
build definition.

Fixes #2081

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 23:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2080" class=".btn">#2080</a>
            </td>
            <td>
                <b>
                    fix(examples): fixed multiple lint errors in examples folder also changed the return types for more functions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Change

1. Fixed lint errors on utility-emissions-channel/enroll-admin-v1-endpoint.ts (line 54, col 25), insert-bamboo-harvest-endpoint.ts (line 78, col 3), insert-bookshelf-endpoint.ts (line 59, col 3), insert-shipment-endpoint.ts (line 69, col 3), list-bamboo-harvest-endpoint.ts (line 38, col 3; line 58, col 3; ), list-bookshelf-endpoint.ts (line 56, col 3), and list-shipment-endpoint.ts (line 40, col 3)
2. In order to fix changes from any to unknown, had to change the output path to directed types: (Changed OASPath return type from any object to "typeof OAS.paths["/api/v1/plugins/@hyperledger/cactus-example-carbon-accounting-backend/dao-token/get-allowance"]"
3. Removed import statements that were never used in the file (import e)
Partial Fix to #1366 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 22:34:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2079" class=".btn">#2079</a>
            </td>
            <td>
                <b>
                    fix(index.ts, emissionsRecordCOntract.ts, get-allowance-endpoint.ts): fixed lint errors on multiple files 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Change
--------------

1. Fixed lint errors on index.ts (line 578, col 25), emissionsRecordContract.ts (line 40, col 3; line 138, col 3; line 146, col 3), and endpoint.ts (line 58, col 33) 
2. In order to fix changes from any to unknown, had to change the output path to directed types: (Changed OASPath return type from any object to "typeof OAS.paths["/api/v1/plugins/@hyperledger/cactus-example-carbon-accounting-backend/dao-token/get-allowance"]"
------------------------------------------------------------
Signed-off-by: Alec Phong <alecphong@gmail.com>
Partial Fix to #1366 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 20:14:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2078" class=".btn">#2078</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha): sending transactions signed on the client-side
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add new endpoint `generate-transaction`, to create unsigned transactions
  that can be signed on the client side.
- Add a function to iroha-connector package to help signing iroha transactions
  on the client (BLP) side.
- Extend transact endpoint to accept signed transaction as an argument as well.
  New transact interface is backward compatible, all current code should work without any change.
- Add new test suite to check features implemented in this PR (i.e. signing on the client side).
- Perform minor cleanup in the connector code, remove unused fields and includes,
  fix some type related warnings.
- Perform openapi interface cleanup, format json correctly,
  mark baseConfig as required by transact (will fail otherwise),
  add error return type schemas, remove invoke-contract endpoint that was not implemented.

Closes #2077

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2076" class=".btn">#2076</a>
            </td>
            <td>
                <b>
                    fix: fixed lint errors pt2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed Lint errors throughout quourum-test-ledger.ts, also fixed a try catch error. 

Partial solution #1375 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 17:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2075" class=".btn">#2075</a>
            </td>
            <td>
                <b>
                    fix: fixed 2 lint errors that were the any type error for Typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed 2 lint errors that were the any type error for Typescript and removed Node
Partial solution to #1375 

Signed-off-by: Alec Phong <alecphong@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 19:01:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2072" class=".btn">#2072</a>
            </td>
            <td>
                <b>
                    docs(build): add text build steps for Linux, Mac and Windows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue: #1963

Signed-off-by: Abhinav Srivastava (abhinavmir#1898 on Discord)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 02:13:32 +0000 UTC
    </div>
</div>

