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
                PR <a href="https://github.com/hyperledger/cactus/pull/2114" class=".btn">#2114</a>
            </td>
            <td>
                <b>
                    build(deps): bump parse-url from 6.0.0 to 6.0.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [parse-url](https://github.com/IonicaBizau/parse-url) from 6.0.0 to 6.0.2.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/IonicaBizau/parse-url/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=parse-url&package-manager=npm_and_yarn&previous-version=6.0.0&new-version=6.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-06 01:44:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2113" class=".btn">#2113</a>
            </td>
            <td>
                <b>
                    test(cactus): remove flaky tests from main CI execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove flaky tests from main CI execution.
- Add separate TAP and jest configuration for running only flaky tests.
- Add test:*:flaky scripts in the main package.json
- Add new step to github CI script to run flaky tests as optional (i.e. don't fail if flaky test fails)

Closes: #2112

Related: #2104
Related: #1626
Related: #2019
Related: #1625
Related: #1543
Related: #1598
Related: #1528
Related: #1521
Related: #1495
Related: #1485
Related: #1473
Related: #1471
Related: #1469
Related: #1150

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 15:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2111" class=".btn">#2111</a>
            </td>
            <td>
                <b>
                    test(connector-sawtooth-socketio): add functional test, bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add functional test of all functions from sawtooth-socketio validator.
- Refactor sawtooth validator to allow importing as a module, to simplify the functional test.
- Add stopMonitor to terminate tests easily.
- Allow multiple clients to monitor for blocks.
- Fix parsing of URL from config so that it doesn't depend on trailing slash anymore.

Closes: https://github.com/hyperledger/cactus/issues/2107

Depends on: https://github.com/hyperledger/cactus/pull/2109
Depends on: https://github.com/hyperledger/cactus/pull/2110
Depends on: https://github.com/hyperledger/cactus/pull/2047

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 18:41:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2110" class=".btn">#2110</a>
            </td>
            <td>
                <b>
                    feat(sawtooth-ledger): add single sawtooth test ledger image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(sawtooth-ledger): add single sawtooth test ledger image

- Enclose starting sawtooth ledger into single container that will fetch and run the entire setup.
- Remove reduntant files, update the readme.
- Add SawtoothTestLedger class to simplify setting the test ledger in jest tests.
- Refactor electricity-trade to generate usage without sawtooth shell patching.
- Refactor electricity-trade to use new sawtooth ledger container and wait until it's healthy.

Closes: https://github.com/hyperledger/cactus/issues/2108

Depends on: https://github.com/hyperledger/cactus/pull/2030

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 18:27:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2109" class=".btn">#2109</a>
            </td>
            <td>
                <b>
                    refactor(connector-sawtooth-socketio): fix strict flag warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cactus-plugin-ledger-connector-sawtooth-socketio will compile with global strict flag.

Related issue: #1671

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 18:26:24 +0000 UTC
    </div>
</div>

