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
                PR <a href="https://github.com/hyperledger/cactus/pull/1848" class=".btn">#1848</a>
            </td>
            <td>
                <b>
                    fix: reset script from package.json does not work #1656
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: #1656

Signed-off-by: ruzell22 <ruzell.vince.aquino@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 03:20:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1847" class=".btn">#1847</a>
            </td>
            <td>
                <b>
                    style(test-tooling): fix unexpected any quorum test ledger start
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Fixes #1844

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 21:34:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1846" class=".btn">#1846</a>
            </td>
            <td>
                <b>
                    style(test-tooling): fix unexpected any quorum test ledger destroy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Fixes #1845

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:12:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1843" class=".btn">#1843</a>
            </td>
            <td>
                <b>
                    refactor(cartrade): upgrade cartrade samples to fabric 2.2 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Add fabcar setup to fabric 2.x all-in-one startup script and adjust
healthcheck accordingly. Use fabric 2.x in cartrade and discounted
cartrade sample apps. No packages updated, fabric sdk 1.4.19 seems to
work fine with fabric 2.2 for now. Both samples has been tested and work
OK.

Closes: https://github.com/hyperledger/cactus/issues/1842
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

### Note: 
- Next step is to use basic asset transfer instead of depracated fabcar, so fabcar-cli-1.4 will be removed in the future (most probably).
- Upgrade of SDK seems to be complex task for now (since packages were re-organized), I think it'd be better to just focus on migration to common fabric connector.

Depends on #1824
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 13:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1841" class=".btn">#1841</a>
            </td>
            <td>
                <b>
                    style: 2021-09-20 linter warnings batch 23/26 fixes: #1371
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the recreation of PR of #1779
 
Reason for this new PR:
The previous repo was deleted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 06:38:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1839" class=".btn">#1839</a>
            </td>
            <td>
                <b>
                    ci: fix CodeQL security scans
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                - Moved the file to the correct directory
- Pinned the runner version to Ubuntu 20.04

Fixes #1836

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 02:49:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1838" class=".btn">#1838</a>
            </td>
            <td>
                <b>
                    build(deps): bump node-fetch from 2.6.6 to 2.6.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [node-fetch](https://github.com/node-fetch/node-fetch) from 2.6.6 to 2.6.7.
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
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/node-fetch/node-fetch/commit/1ef4b560a17e644a02a3bfdea7631ffeee578b35"><code>1ef4b56</code></a> backport of <a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1449">#1449</a> (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1453">#1453</a>)</li>
<li><a href="https://github.com/node-fetch/node-fetch/commit/8fe5c4ea66b9b8187600e6d5ec9b1b6781f44009"><code>8fe5c4e</code></a> 2.x: Specify encoding as an optional peer dependency in package.json (<a href="https://github-redirect.dependabot.com/node-fetch/node-fetch/issues/1310">#1310</a>)</li>
<li>See full diff in <a href="https://github.com/node-fetch/node-fetch/compare/v2.6.6...v2.6.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=node-fetch&package-manager=npm_and_yarn&previous-version=2.6.6&new-version=2.6.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-02-04 06:24:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1837" class=".btn">#1837</a>
            </td>
            <td>
                <b>
                    build(deps): bump simple-get from 2.8.1 to 2.8.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 2.8.1 to 2.8.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/4e156b6bb19e11ccfad05fad310ea799d63f890d"><code>4e156b6</code></a> 2.8.2</li>
<li><a href="https://github.com/feross/simple-get/commit/43c272db3e4b1383cb03d80338dba3e08c451641"><code>43c272d</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v2.8.1...v2.8.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=2.8.1&new-version=2.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-02-04 06:24:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1835" class=".btn">#1835</a>
            </td>
            <td>
                <b>
                    test: jestify plugin-keychain-memory test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                
Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-keychain-memory/src/
test/typescript/unit/plugin-keychain-memory.test.ts

This is a PARTIAL resolution to issue https://github.com/hyperledger/cactus/issues/238

Signed-off-by: awadhana <awadhana2021@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 14:25:25 +0000 UTC
    </div>
</div>

