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
                PR <a href="https://github.com/hyperledger/cactus/pull/2066" class=".btn">#2066</a>
            </td>
            <td>
                <b>
                    build(deps): bump eventsource from 1.1.0 to 1.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [eventsource](https://github.com/EventSource/eventsource) from 1.1.0 to 1.1.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/EventSource/eventsource/blob/master/HISTORY.md">eventsource's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">1.1.1</a></h1>
<ul>
<li>Do not include authorization and cookie headers on redirect to different origin (<a href="https://github-redirect.dependabot.com/EventSource/eventsource/pull/273">#273</a> Espen Hovlandsdal)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/EventSource/eventsource/commit/aa7a40843a978f42c0babdec125bf9e0a83bf515"><code>aa7a408</code></a> 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/56d489ef853a891deca121bbd463c732fee94dce"><code>56d489e</code></a> chore: rebuild polyfill</li>
<li><a href="https://github.com/EventSource/eventsource/commit/4a951e58b04118c9c4d3da3d27d454972a1b4b8d"><code>4a951e5</code></a> docs: update history for 1.1.1</li>
<li><a href="https://github.com/EventSource/eventsource/commit/f9f6416567bff62c1af2f4314be51d9870e94bc2"><code>f9f6416</code></a> fix: strip sensitive headers on redirect to different origin</li>
<li>See full diff in <a href="https://github.com/EventSource/eventsource/compare/v1.1.0...v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=eventsource&package-manager=npm_and_yarn&previous-version=1.1.0&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-01 22:29:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2053" class=".btn">#2053</a>
            </td>
            <td>
                <b>
                    test(connector-go-ethereum-socketio): add functional test, bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add functional test of all functions from go-ethereum-socketio validator.
- Refactor go-ethereum validator to allow importing as a module, to simplify the functional test.
- Fix sendRawTransaction to work with Verifier protocol.
  It couldn't be reached by any client library until now, so I consider this as "private" interface.
- Add common web3 client object in openethereum test ledger helper class.
- Add few new functions to ethereum test ledger helper class:
  newEthPersonalAccount, transferAssetFromCoinbase, deployContract.

Depends on #2051
Depends on #2047

Closes: #2052

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

-------------

Please consider only the last commit - `test(connector-go-ethereum-socketio): add functional test, bug fix`. The rest are the dependencies that should be merged by separate PRs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 09:57:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2051" class=".btn">#2051</a>
            </td>
            <td>
                <b>
                    refactor(connector-go-ethereum-socketio): fix strict flag warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cactus-plugin-ledger-connector-go-ethereum-socketio will compile with global strict flag.

Related issue: #1671

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 08:56:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2050" class=".btn">#2050</a>
            </td>
            <td>
                <b>
                    build(openapi): generate kotlin client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
---------------------------------

build(openapi): generate kotlin client

    Primary Changes
    ---------------
    1. Updated the root package.json and cactus-plugin-ledger-connector-corda
 	   package.json to incorporate generate-clients script
    2. Created a git action workflow to generate version-tagged client artifacts

Fixes #2000

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 07:44:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2049" class=".btn">#2049</a>
            </td>
            <td>
                <b>
                    test: jestify invoke contract in connector besu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrate Tap to Jest

File Path:
packages/cactus-plugin-ledger-connector-besu/
src/test/typescript/
integration/plugin-ledger-connector-besu/
deploy-contract/
invoke-contract.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 13:18:15 +0000 UTC
    </div>
</div>

