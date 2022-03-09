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
                PR <a href="https://github.com/hyperledger/cactus/pull/1903" class=".btn">#1903</a>
            </td>
            <td>
                <b>
                    test(cmd-api-server): fix flaky runtime-plugin-imports-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a flaky test case that can't be reliably reproduce. I've ran the test individually 40 times and all 40 times it has passed successfully. 

This error, however, seems to pop up only when the `yarn jest` command is run (when I ran the test individually). 

Based on the linked ["hint"](https://stackoverflow.com/questions/50793885/referenceerror-you-are-trying-to-import-a-file-after-the-jest-environment-has/50793993#50793993) from the issue, it seems like using `jest.useFakeTimers()` a good solution. However, using the `jest.useFakeTimers()` with`async/await` was not recommended.

However, I found a [different source](https://gist.github.com/apieceofbart/e6dea8d884d29cf88cdb54ef14ddbcc4#file-test-js-L58) that showed examples of how to use the `jest.useFakeTimers()`. Our original problem, however, is probably because the after the test environment is torn down, the second test file is trying to import files from the first environment, triggering the error ([explained here](https://github.com/facebook/jest/issues/11438#issuecomment-916711164)). So I've come to the solution of installing another node package: [node-cleanup](https://www.npmjs.com/package/node-cleanup) and running that within the afterAll at the very end of the test. 

My laptop can't take running the `yarn jest` script too much so I haven't seen it reproduce the error yet. (WOT ruhrow) 

Fixes #1667 
 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 21:26:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1902" class=".btn">#1902</a>
            </td>
            <td>
                <b>
                    refactor(plugin-odap-gateway): refactor implementation including more tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Rename plugin file from **odap-gateway** to **plugin-odap-gateway**.
* Refactor **SendClientRequest()** 600 lines method into different methods according to the ODAP phase and each message type.
* Refactor methods that make digital signatures and respective verification.
* Added tests and actual verification regarding the state of the objects.
* Added fields in the open API file according to the specification in the ODAP draft.
* Added checks in every step of the protocol according to the messages exchanged

cc @RafaelAPB 

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 19:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1901" class=".btn">#1901</a>
            </td>
            <td>
                <b>
                    docs(whitepaper): update whitepaper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Our whitepaper, the first point of contact from enterprises and individuals alike, is very outdated (for more than two years, it received no updates).  An outdated whitepaper brings a lot of confusion to newcomers, as 1) it doesn' reflect updated work done on blockchain interoperability, 2) doesn't reflect the current status of the code, and 3) doesn't reflect future plans for the project

These problems have been and continue to hamper the adoption of Hyperledger Cacuts.

I'm putting together an effort to update the whitepaper, with an initial focus on the abstract, introduction, and theoretical models (non-formal) for interoperability (based on [our recent research](https://www.techrxiv.org/articles/preprint/Do_You_Need_a_Distributed_Ledger_Technology_Interoperability_Solution_/18786527/1)). 

I welcome all the blockchain interoperability and Hyperledger's communities to provide their feedback to this new version of the whitepaper.

Changes:

1. Updated abstract
2. Introduction now explains why do we need interoperability, Cactus, and how Cactus works
3. Section 2 now contains a robust model for interoperability. Some outdated information was refactored.
4. Updated references and recommended reference to the project (feel free to add yourself!)  

cc @petermetz @takeutak @sfuji822 @jagpreetsinghsasan @jonathan-m-hamilton @hartm 

Signed-off-by: Rafael Belchior <rafael.belchior@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 12:44:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1900" class=".btn">#1900</a>
            </td>
            <td>
                <b>
                    refactor: migrate to jest and fix neg test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Original issue was to  __test(plugin-htlc-eth-besu): fix assertion withdraw-endpoint-invalid #1871__  However, this test case hadn't been jestified (slipped through the cracks according to @awadhana) so I went ahead and jestified the file along with fixing the negative test case. Commit message for jestification and the original issue. 

_______________________________
Migrated test from Tap to Jest

File Path: packages/cactus-test-plugin-htlc-eth-besu/src/test/typescript/integration/plugin-htlc-eth-besu/withdraw-endpoint-invalid.test.ts
This is a PARTIAL resolution to issue https://github.com/hyperledger/cactus/issues/238
_______________________________

Fixes #1871 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 20:10:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1896" class=".btn">#1896</a>
            </td>
            <td>
                <b>
                    refactor(cmd-socketio): validators should be configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add the possibility to adjust connector behavior through separate config file.
- Use node-config package for configuration management.
- Add helper classes in validators for easy config entry retrieval.
- Remove obsolete and unnecessary components.
- Adjust sample applications to work in current setup.

Closes: #1895
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

Note - the changes are very similar in all 3 affected ledger connectors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 14:31:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1893" class=".btn">#1893</a>
            </td>
            <td>
                <b>
                    docs: minor tweaks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                -add mention to test running via interface
-explain in more detail the docker requirement
-fix small bug preventing the correct execution of generate-api-server

cc @petermetz 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 14:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1892" class=".btn">#1892</a>
            </td>
            <td>
                <b>
                    test: jestify jwt-unprotected-endpoint-authz-ops-confirm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest

File Path:
packages/cactus-cmd-api-server/src/test/typescript/
integration/jwt-unprotected-endpoint-authz-ops-confirm.test.ts

This is a PARTIAL resolution to issue hyperledger#238

NOT ready to merge, I need to correct the way .toRejects() happens


Signed-off-by: awadhana <awadhana2021@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 00:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1891" class=".btn">#1891</a>
            </td>
            <td>
                <b>
                    test(get-single-status-endpoint-invalid): jestify get-single-status-endpoint-invalid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/get-single-status-endpoint-invalid.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana2021@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 23:20:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1889" class=".btn">#1889</a>
            </td>
            <td>
                <b>
                    Cactus test plugin htlc eth besu erc20/withdraw endpoint invalid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/withdraw-endpoint-invalid-id.test.ts

This is a PARTIAL resolution to issue https://github.com/hyperledger/cactus/issues/238

Signed-off-by: awadhana <awadhana2021@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 19:07:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1888" class=".btn">#1888</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump karma from 6.3.14 to 6.3.16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [karma](https://github.com/karma-runner/karma) from 6.3.14 to 6.3.16.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/karma-runner/karma/releases">karma's releases</a>.</em></p>
<blockquote>
<h2>v6.3.16</h2>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.15...v6.3.16">6.3.16</a> (2022-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> mitigate the &quot;Open Redirect Vulnerability&quot; (<a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d">ff7edbb</a>)</li>
</ul>
<h2>v6.3.15</h2>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.15">6.3.15</a> (2022-02-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>helper:</strong> make mkdirIfNotExists helper resilient to concurrent calls (<a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404">d9dade2</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/karma-runner/karma-coverage/issues/434/issues/issuecomment-1017939333">karma-runner/karma-coverage#434</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/karma-runner/karma/blob/master/CHANGELOG.md">karma's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.15...v6.3.16">6.3.16</a> (2022-02-10)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>security:</strong> mitigate the &quot;Open Redirect Vulnerability&quot; (<a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d">ff7edbb</a>)</li>
</ul>
<h2><a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.15">6.3.15</a> (2022-02-05)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>helper:</strong> make mkdirIfNotExists helper resilient to concurrent calls (<a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404">d9dade2</a>), closes <a href="https://github-redirect.dependabot.com//github-redirect.dependabot.com/karma-runner/karma-coverage/issues/434/issues/issuecomment-1017939333">karma-runner/karma-coverage#434</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/karma-runner/karma/commit/ab4b32898bcb4e0ba3a1e99835d30c113db3eeeb"><code>ab4b328</code></a> chore(release): 6.3.16 [skip ci]</li>
<li><a href="https://github.com/karma-runner/karma/commit/ff7edbb2ffbcdd69761bece86b7dc1ef0740508d"><code>ff7edbb</code></a> fix(security): mitigate the &quot;Open Redirect Vulnerability&quot;</li>
<li><a href="https://github.com/karma-runner/karma/commit/c1befa04b32b90f088fefdc0521c6f48cbc510a9"><code>c1befa0</code></a> chore(release): 6.3.15 [skip ci]</li>
<li><a href="https://github.com/karma-runner/karma/commit/d9dade2f004a340e49c9a633177576200c286404"><code>d9dade2</code></a> fix(helper): make mkdirIfNotExists helper resilient to concurrent calls</li>
<li><a href="https://github.com/karma-runner/karma/commit/653c762be4fa464fed5bfa306317b84cc5c28a17"><code>653c762</code></a> ci: prevent duplicate CI tasks on creating a PR</li>
<li>See full diff in <a href="https://github.com/karma-runner/karma/compare/v6.3.14...v6.3.16">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=karma&package-manager=npm_and_yarn&previous-version=6.3.14&new-version=6.3.16)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-02 13:39:37 +0000 UTC
    </div>
</div>

