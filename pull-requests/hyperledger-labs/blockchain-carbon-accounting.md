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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/351" class=".btn">#351</a>
            </td>
            <td>
                <b>
                    eth-identity: add ethereum integration with vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow ethereum private key for signing cross-ledger transactions in Cactus.

close #277 

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 17:19:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/350" class=".btn">#350</a>
            </td>
            <td>
                <b>
                    build(deps): bump keypair from 1.0.2 to 1.0.4 in /net-emissions-token-network/interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [keypair](https://github.com/juliangruber/keypair) from 1.0.2 to 1.0.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/juliangruber/keypair/releases">keypair's releases</a>.</em></p>
<blockquote>
<h2>v1.0.4</h2>
<ul>
<li>Merge pull request from GHSA-3f99-hvg4-qjwj  9596418</li>
</ul>
<p><a href="https://github.com/juliangruber/keypair/compare/v1.0.3...v1.0.4">https://github.com/juliangruber/keypair/compare/v1.0.3...v1.0.4</a></p>
<h2>v1.0.3</h2>
<ul>
<li>pkg: clean up  89dafaa</li>
<li>fix:typescript: set default export (<a href="https://github-redirect.dependabot.com/juliangruber/keypair/issues/18">#18</a>)  b0360f6</li>
</ul>
<p><a href="https://github.com/juliangruber/keypair/compare/v1.0.2...v1.0.3">https://github.com/juliangruber/keypair/compare/v1.0.2...v1.0.3</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/juliangruber/keypair/commit/65f9f24c561c73e37b408310d6c07ee50af0f575"><code>65f9f24</code></a> 1.0.4</li>
<li><a href="https://github.com/juliangruber/keypair/commit/9596418d3363d3e757676c0b6a8f2d35a9d1cb18"><code>9596418</code></a> Merge pull request from GHSA-3f99-hvg4-qjwj</li>
<li><a href="https://github.com/juliangruber/keypair/commit/87c62f255baa12c1ec4f98a91600f82af80be6db"><code>87c62f2</code></a> 1.0.3</li>
<li><a href="https://github.com/juliangruber/keypair/commit/89dafaa3475419c847bab75b390f73f6f4a2e220"><code>89dafaa</code></a> pkg: clean up</li>
<li><a href="https://github.com/juliangruber/keypair/commit/b0360f6367947fab9476b7be387146100fd59e4f"><code>b0360f6</code></a> fix:typescript: set default export (<a href="https://github-redirect.dependabot.com/juliangruber/keypair/issues/18">#18</a>)</li>
<li>See full diff in <a href="https://github.com/juliangruber/keypair/compare/v1.0.2...v1.0.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=keypair&package-manager=npm_and_yarn&previous-version=1.0.2&new-version=1.0.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-05 16:35:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/349" class=".btn">#349</a>
            </td>
            <td>
                <b>
                    build(deps): bump url-parse from 1.5.1 to 1.5.3 in /open-offsets-directory/react
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [url-parse](https://github.com/unshiftio/url-parse) from 1.5.1 to 1.5.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/unshiftio/url-parse/commit/ad444931666a30bad11472d89a216461cf16cae2"><code>ad44493</code></a> [dist] 1.5.3</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/c7984617e235892cc22e0f47bb5ff1c012e6e39f"><code>c798461</code></a> [fix] Fix host parsing for file URLs (<a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/210">#210</a>)</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/201034b8670c2aa382d7ec410ee750ac6f2f9c38"><code>201034b</code></a> [dist] 1.5.2</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/2d9ac2c94067742b2116332c1e03be9f37371dff"><code>2d9ac2c</code></a> [fix] Sanitize only special URLs (<a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/209">#209</a>)</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/fb128af4f43fa17f351d50cf615c7598c751f50a"><code>fb128af</code></a> [fix] Use <code>'null'</code> as <code>origin</code> for non special URLs</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/fed6d9e338ea39de2d68bb66607066d71328c62f"><code>fed6d9e</code></a> [fix] Add a leading slash only if the URL is special</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/94872e7ab9103ee69b958959baa14c9e682a7f10"><code>94872e7</code></a> [fix] Do not incorrectly set the <code>slashes</code> property to <code>true</code></li>
<li><a href="https://github.com/unshiftio/url-parse/commit/81ab967889b08112d3356e451bf03e6aa0cbb7e0"><code>81ab967</code></a> [fix] Ignore slashes after the protocol for special URLs</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ee22050a48a67409aa5f7c87947284156d615bd1"><code>ee22050</code></a> [ci] Use GitHub Actions</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/d2979b586d8c7751e0c77f127d9ce1b2143cc0c9"><code>d2979b5</code></a> [fix] Special case the <code>file:</code> protocol (<a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/204">#204</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/unshiftio/url-parse/compare/1.5.1...1.5.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url-parse&package-manager=npm_and_yarn&previous-version=1.5.1&new-version=1.5.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-11-05 16:34:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/348" class=".btn">#348</a>
            </td>
            <td>
                <b>
                    identity(ui): add identity-ui for vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #313 

Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 11:38:09 +0000 UTC
    </div>
</div>

