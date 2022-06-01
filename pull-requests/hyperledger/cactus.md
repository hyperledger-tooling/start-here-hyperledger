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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2048" class=".btn">#2048</a>
            </td>
            <td>
                <b>
                    feat(iroha-connector): implement validator interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(iroha-connector): implement validator interface

Add monitoring and sending async/sync requests to ledger via SocketIO.

Closes: https://github.com/hyperledger/cactus/issues/1941

Author: stepniowskip <piotr.stepniowski@fujitsu.com>

Original PR: #1966
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 11:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2047" class=".btn">#2047</a>
            </td>
            <td>
                <b>
                    refactor(cmd-socketio-server): remove code duplication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Moved verifyValidatorJwt to `cactus-common` to keep encrypt/decrypt logic
  of socketio-based validators in one, common location.
- Move config-reading and signMessageJwt helper functions from validators to cmd-socketio-server
  to remove code duplication.
  Refactor validators to use these common instead of own implementation.
- Remove ValidatorAuthentication.ts that is not used anymore
  (not part of public interface, it was copied by validators during before couple commits ago).
- Create jwt-message-authentication.test.ts from old, similar one in cactus-api-client.
- Updated readme with instructions of how to start asset-trade and electricity-trade samples
  without docker-compose (to be used during development).
  Added helper script for patching the config.

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

-----------------

This PR is for the last commit only - [refactor(cmd-socketio-server): remove code duplication](https://github.com/hyperledger/cactus/commit/200a7da23d68a38eb2c1af8869175e172c1d3b62). Please ignore previous one (dependencies) which will be removed before the merge.

Depends on #2033
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 10:56:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2046" class=".btn">#2046</a>
            </td>
            <td>
                <b>
                    build(deps): bump convict from 6.2.2 to 6.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [convict](https://github.com/mozilla/node-convict) from 6.2.2 to 6.2.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/mozilla/node-convict/blob/master/CHANGELOG.md">convict's changelog</a>.</em></p>
<blockquote>
<h2>[6.2.3] - 2022-05-07</h2>
<h3>Fixed</h3>
<ul>
<li>More more complete fix for prototype pollution vulnerability first addressed
in <a href="https://github-redirect.dependabot.com/mozilla/node-convict/issues/384">#384</a> (Marc-Aurèle Darche <a href="https://github.com/madarche"><code>@​madarche</code></a>, Snyk Security team)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/mozilla/node-convict/commit/deef5d77f4f6a714579387c2d67a051396477415"><code>deef5d7</code></a> v6.2.3</li>
<li><a href="https://github.com/mozilla/node-convict/commit/5e64b53082628abb9e4888838fcc8fe2851395ee"><code>5e64b53</code></a> More recent Ubuntu dist for Travis CI build</li>
<li><a href="https://github.com/mozilla/node-convict/commit/1ea0ab19c5208f66509e1c43b0d0f21c1fd29b75"><code>1ea0ab1</code></a> More more complete fix for prototype pollution</li>
<li><a href="https://github.com/mozilla/node-convict/commit/c7acb024c592652a6ad7f94ff7beed1df2d477ad"><code>c7acb02</code></a> Update info regarding publishing on NPM</li>
<li>See full diff in <a href="https://github.com/mozilla/node-convict/compare/v6.2.2...v6.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=convict&package-manager=npm_and_yarn&previous-version=6.2.2&new-version=6.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-05-26 03:00:08 +0000 UTC
    </div>
</div>

