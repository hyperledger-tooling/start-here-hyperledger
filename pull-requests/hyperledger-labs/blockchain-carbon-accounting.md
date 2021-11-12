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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    REST API for ws-wallet web-socket-key request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ws-wallet REST API to request and authorize web-socket keys for third party applications

POST /session/new/ ,
body: {endpoint: <fabric app's ws-identity session ticket  url>, key_name: <keyName>}

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 03:56:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/356" class=".btn">#356</a>
            </td>
            <td>
                <b>
                    feat(CI): Add tests for net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added tests for `net-emissions-token-network` to the CI pipeline. @udosson as for uploading the test results, `npx hardhat test` does not provide any options as of now to export the test results, even though they are internally using Mocha. So, for the moment, it won't be possible to upload the test reports as an artifact to get the test reports using the `test-reporter` action. We could request the feature to export test reports [on their repo](https://github.com/nomiclabs/hardhat), or I could work on this if needed in the future.

Closes #292.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 11:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/355" class=".btn">#355</a>
            </td>
            <td>
                <b>
                    docs(CI): Add comments for CI pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added in-line comments to the YAML workflow files for the CI pipeline. Closes #307.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 07:13:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/354" class=".btn">#354</a>
            </td>
            <td>
                <b>
                    Add password encryption to PKCS#8 private key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    - ws-wallet new-key requests user to input password to encrypt PKCS#8 private key
    - ws-wallet open will request password to decrypt private key for signing
    - getPass() fn handles terminal requests to input passwor 
    - unlockKey() fn checks if decryption password is valid. Process closed after 3 failed attempts
    - Password -p option can be provided with new-key and open commands

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-06 21:05:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/353" class=".btn">#353</a>
            </td>
            <td>
                <b>
                    build(deps): bump ws from 5.2.2 to 5.2.3 in /net-emissions-token-network/interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [ws](https://github.com/websockets/ws) from 5.2.2 to 5.2.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>5.2.3</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported 00c425ec to the 5.x release line (76d47c14).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/6dd88e7e968ef2416445d8f8620c17d99b15c77c"><code>6dd88e7</code></a> [dist] 5.2.3</li>
<li><a href="https://github.com/websockets/ws/commit/76d47c1479002022a3e4357b3c9f0e23a68d4cd2"><code>76d47c1</code></a> [security] Fix ReDoS vulnerability</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/5.2.2...5.2.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ws&package-manager=npm_and_yarn&previous-version=5.2.2&new-version=5.2.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-05 20:33:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/352" class=".btn">#352</a>
            </td>
            <td>
                <b>
                    typeo_fix: fixed in vault-identity and identity-ui
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed small typo fix in `vault-identity` and `identity-ui`
Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 20:08:19 +0000 UTC
    </div>
</div>

