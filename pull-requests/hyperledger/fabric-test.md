---
layout: default
title: fabric-test
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-test
---

# fabric-test <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-test){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    Disable daily test for release-2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                release-2.3 will not be updated to Go 1.18, therefore disable
the test to suppress failures related to Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 11:17:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    Fix branches for hsm docker images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix branches for hsm docker images to use release-2.4.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-03 20:23:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/390" class=".btn">#390</a>
            </td>
            <td>
                <b>
                    Turn off test-release pipeline for release-2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Turn off test-release pipeline for release-2.0

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-03 20:18:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/389" class=".btn">#389</a>
            </td>
            <td>
                <b>
                    Run interop and daily pipelines on supported releases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Only run interop and daily pipelines on:
        - main
        - release-2.4
        - release-2.2

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-03 20:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/388" class=".btn">#388</a>
            </td>
            <td>
                <b>
                    Bump protobufjs from 6.11.2 to 6.11.3 in /tools/chaincode-integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.11.2 to 6.11.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/releases">protobufjs's releases</a>.</em></p>
<blockquote>
<h2>v6.11.3</h2>
<h3><a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.2...v6.11.3">6.11.3</a> (2022-05-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea">a8681ce</a>)</li>
<li>do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f">b5f1391</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/protobufjs/protobuf.js/blob/v6.11.3/CHANGELOG.md">protobufjs's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.2...v6.11.3">6.11.3</a> (2022-05-20)</h3>
<h3>Bug Fixes</h3>
<ul>
<li><strong>deps:</strong> use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea">a8681ce</a>)</li>
<li>do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>) (<a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f">b5f1391</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b130dfd4f06b642d4b7c3ccc9f3f9fb6a6e6ed0d"><code>b130dfd</code></a> chore(6.x): release 6.11.3 (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1737">#1737</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/c2c17ae66810378fbad616964d80894794f1dad1"><code>c2c17ae</code></a> build: publish to main</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b2c6a5c76eccd4bbe445d13e3a04b949f344dd63"><code>b2c6a5c</code></a> build: run tests if ci label added (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1734">#1734</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/a8681ceab4763e706a848121a2dde56791b89eea"><code>a8681ce</code></a> fix(deps): use eslint 8.x (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1728">#1728</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/b5f1391dff5515894830a6570e6d73f5511b2e8f"><code>b5f1391</code></a> fix: do not let setProperty change the prototype (<a href="https://github-redirect.dependabot.com/protobufjs/protobuf.js/issues/1731">#1731</a>)</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/7afd0a39f41d6df5fda6fa10c319cdf829027d3e"><code>7afd0a3</code></a> build: configure 6.x as default branch</li>
<li><a href="https://github.com/protobufjs/protobuf.js/commit/37285d0cdc8b20acacd0227daa2e577921de46a7"><code>37285d0</code></a> build: configure backports</li>
<li>See full diff in <a href="https://github.com/protobufjs/protobuf.js/compare/v6.11.2...v6.11.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.11.2&new-version=6.11.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-test/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-03 01:45:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/387" class=".btn">#387</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.2

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 18:25:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/386" class=".btn">#386</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.2

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 18:24:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/384" class=".btn">#384</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.2.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 15:40:44 +0000 UTC
    </div>
</div>

