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
                PR <a href="https://github.com/hyperledger/cactus/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    chore(deps): bump ssri from 6.0.1 to 6.0.2 in /packages/cactus-cockpit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #849

Bumps [ssri](https://github.com/npm/ssri) from 6.0.1 to 6.0.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/ssri/blob/v6.0.2/CHANGELOG.md">ssri's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/zkat/ssri/compare/v6.0.1...v6.0.2">6.0.2</a> (2021-04-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>backport regex change from 8.0.1 (<a href="https://github.com/zkat/ssri/commit/b30dfdb">b30dfdb</a>), closes <a href="https://github-redirect.dependabot.com/zkat/ssri/issues/19">#19</a></li>
</ul>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/ssri/commit/b7c8c7c61db89aeb9fbf7596c0ef17071bc216ef"><code>b7c8c7c</code></a> chore(release): 6.0.2</li>
<li><a href="https://github.com/npm/ssri/commit/b30dfdb00bb94ddc49a25a85a18fb27afafdfbb1"><code>b30dfdb</code></a> fix: backport regex change from 8.0.1</li>
<li>See full diff in <a href="https://github.com/npm/ssri/compare/v6.0.1...v6.0.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~nlf">nlf</a>, a new releaser for ssri since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ssri&package-manager=npm_and_yarn&previous-version=6.0.1&new-version=6.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-04-20 02:22:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): contract deployment with constructor arguments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">enhancement</span>
            </td>
            <td>
                Previously you couldn't deploy a contract that had constructor arguments
of it's own because there was no way to pass in these.
With this improvement this is now possible.

Depends on #810

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

cc: @jordigiam @AzaharaC 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 21:55:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-test-api-client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #849

Bumps [jose](https://github.com/panva/jose) from 1.27.2 to 1.28.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v1.28.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>), fixes <a href="https://github.com/panva/jose/security/advisories/GHSA-58f5-hfqc-jgch">CVE-2021-29443</a></li>
</ul>
<h2>v1.28.0</h2>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2>v1.27.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/v1.28.1/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/panva/jose/compare/v1.28.0...v1.28.1">1.28.1</a> (2021-04-09)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>)</li>
</ul>
<h1><a href="https://github.com/panva/jose/compare/v1.27.3...v1.28.0">1.28.0</a> (2020-08-10)</h1>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v1.27.2...v1.27.3">1.27.3</a> (2020-08-04)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/51e0d8b3fbc1faebf67f6dbaced1095534d7017f"><code>51e0d8b</code></a> chore(release): 1.28.1</li>
<li><a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b"><code>08e1bc5</code></a> fix: defer AES CBC w/ HMAC decryption after tag verification passes</li>
<li><a href="https://github.com/panva/jose/commit/9a8404a7592c3d56093a3bf31a4ab263721ed644"><code>9a8404a</code></a> chore(release): 1.28.0</li>
<li><a href="https://github.com/panva/jose/commit/eb482a8ab825bb54dc0a89d55b1ffc7bf6bd24f4"><code>eb482a8</code></a> style: lib/jwe/encrypt.js</li>
<li><a href="https://github.com/panva/jose/commit/e0a2d579269a4787ba997bfac9b58d641ff9fa04"><code>e0a2d57</code></a> refactor: sign.js PROCESS_RECIPIENT</li>
<li><a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13"><code>ce6836a</code></a> feat: support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>)</li>
<li><a href="https://github.com/panva/jose/commit/db6254e575e6fbc0a564b80ed9e488628187a25e"><code>db6254e</code></a> ci: improve CI runtime</li>
<li><a href="https://github.com/panva/jose/commit/1a4a68fb9a2ab5e2b796545482a4d8f1a5e6e6b7"><code>1a4a68f</code></a> chore(release): 1.27.3</li>
<li><a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4"><code>d56ec9f</code></a> fix: ensure &quot;b64&quot; is the same for all recipients edge cases</li>
<li><a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469"><code>1695423</code></a> fix: do not mutate unencoded payload when signing for multiple parties</li>
<li>Additional commits viewable in <a href="https://github.com/panva/jose/compare/v1.27.2...v1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=1.27.2&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-04-19 15:03:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/822" class=".btn">#822</a>
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-test-cmd-api-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #849

Bumps [jose](https://github.com/panva/jose) from 1.27.2 to 1.28.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v1.28.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>), fixes <a href="https://github.com/panva/jose/security/advisories/GHSA-58f5-hfqc-jgch">CVE-2021-29443</a></li>
</ul>
<h2>v1.28.0</h2>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2>v1.27.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/v1.28.1/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/panva/jose/compare/v1.28.0...v1.28.1">1.28.1</a> (2021-04-09)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>)</li>
</ul>
<h1><a href="https://github.com/panva/jose/compare/v1.27.3...v1.28.0">1.28.0</a> (2020-08-10)</h1>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v1.27.2...v1.27.3">1.27.3</a> (2020-08-04)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/51e0d8b3fbc1faebf67f6dbaced1095534d7017f"><code>51e0d8b</code></a> chore(release): 1.28.1</li>
<li><a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b"><code>08e1bc5</code></a> fix: defer AES CBC w/ HMAC decryption after tag verification passes</li>
<li><a href="https://github.com/panva/jose/commit/9a8404a7592c3d56093a3bf31a4ab263721ed644"><code>9a8404a</code></a> chore(release): 1.28.0</li>
<li><a href="https://github.com/panva/jose/commit/eb482a8ab825bb54dc0a89d55b1ffc7bf6bd24f4"><code>eb482a8</code></a> style: lib/jwe/encrypt.js</li>
<li><a href="https://github.com/panva/jose/commit/e0a2d579269a4787ba997bfac9b58d641ff9fa04"><code>e0a2d57</code></a> refactor: sign.js PROCESS_RECIPIENT</li>
<li><a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13"><code>ce6836a</code></a> feat: support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>)</li>
<li><a href="https://github.com/panva/jose/commit/db6254e575e6fbc0a564b80ed9e488628187a25e"><code>db6254e</code></a> ci: improve CI runtime</li>
<li><a href="https://github.com/panva/jose/commit/1a4a68fb9a2ab5e2b796545482a4d8f1a5e6e6b7"><code>1a4a68f</code></a> chore(release): 1.27.3</li>
<li><a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4"><code>d56ec9f</code></a> fix: ensure &quot;b64&quot; is the same for all recipients edge cases</li>
<li><a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469"><code>1695423</code></a> fix: do not mutate unencoded payload when signing for multiple parties</li>
<li>Additional commits viewable in <a href="https://github.com/panva/jose/compare/v1.27.2...v1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=1.27.2&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-04-19 15:03:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/821" class=".btn">#821</a>
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-test-plugin-consortium-manual
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #849

Bumps [jose](https://github.com/panva/jose) from 1.27.2 to 1.28.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v1.28.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>), fixes <a href="https://github.com/panva/jose/security/advisories/GHSA-58f5-hfqc-jgch">CVE-2021-29443</a></li>
</ul>
<h2>v1.28.0</h2>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2>v1.27.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/v1.28.1/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/panva/jose/compare/v1.28.0...v1.28.1">1.28.1</a> (2021-04-09)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>)</li>
</ul>
<h1><a href="https://github.com/panva/jose/compare/v1.27.3...v1.28.0">1.28.0</a> (2020-08-10)</h1>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v1.27.2...v1.27.3">1.27.3</a> (2020-08-04)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/51e0d8b3fbc1faebf67f6dbaced1095534d7017f"><code>51e0d8b</code></a> chore(release): 1.28.1</li>
<li><a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b"><code>08e1bc5</code></a> fix: defer AES CBC w/ HMAC decryption after tag verification passes</li>
<li><a href="https://github.com/panva/jose/commit/9a8404a7592c3d56093a3bf31a4ab263721ed644"><code>9a8404a</code></a> chore(release): 1.28.0</li>
<li><a href="https://github.com/panva/jose/commit/eb482a8ab825bb54dc0a89d55b1ffc7bf6bd24f4"><code>eb482a8</code></a> style: lib/jwe/encrypt.js</li>
<li><a href="https://github.com/panva/jose/commit/e0a2d579269a4787ba997bfac9b58d641ff9fa04"><code>e0a2d57</code></a> refactor: sign.js PROCESS_RECIPIENT</li>
<li><a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13"><code>ce6836a</code></a> feat: support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>)</li>
<li><a href="https://github.com/panva/jose/commit/db6254e575e6fbc0a564b80ed9e488628187a25e"><code>db6254e</code></a> ci: improve CI runtime</li>
<li><a href="https://github.com/panva/jose/commit/1a4a68fb9a2ab5e2b796545482a4d8f1a5e6e6b7"><code>1a4a68f</code></a> chore(release): 1.27.3</li>
<li><a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4"><code>d56ec9f</code></a> fix: ensure &quot;b64&quot; is the same for all recipients edge cases</li>
<li><a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469"><code>1695423</code></a> fix: do not mutate unencoded payload when signing for multiple parties</li>
<li>Additional commits viewable in <a href="https://github.com/panva/jose/compare/v1.27.2...v1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=1.27.2&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-04-19 15:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/820" class=".btn">#820</a>
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.28.0 to 1.28.1 in /examples/cactus-example-supply-chain-backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #849

Bumps [jose](https://github.com/panva/jose) from 1.28.0 to 1.28.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v1.28.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>), fixes <a href="https://github.com/panva/jose/security/advisories/GHSA-58f5-hfqc-jgch">CVE-2021-29443</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/v1.28.1/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/panva/jose/compare/v1.28.0...v1.28.1">1.28.1</a> (2021-04-09)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/51e0d8b3fbc1faebf67f6dbaced1095534d7017f"><code>51e0d8b</code></a> chore(release): 1.28.1</li>
<li><a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b"><code>08e1bc5</code></a> fix: defer AES CBC w/ HMAC decryption after tag verification passes</li>
<li>See full diff in <a href="https://github.com/panva/jose/compare/v1.28.0...v1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=1.28.0&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-04-19 15:02:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/819" class=".btn">#819</a>
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-cmd-api-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #849

Bumps [jose](https://github.com/panva/jose) from 1.27.2 to 1.28.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v1.28.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>), fixes <a href="https://github.com/panva/jose/security/advisories/GHSA-58f5-hfqc-jgch">CVE-2021-29443</a></li>
</ul>
<h2>v1.28.0</h2>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2>v1.27.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/v1.28.1/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/panva/jose/compare/v1.28.0...v1.28.1">1.28.1</a> (2021-04-09)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>)</li>
</ul>
<h1><a href="https://github.com/panva/jose/compare/v1.27.3...v1.28.0">1.28.0</a> (2020-08-10)</h1>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v1.27.2...v1.27.3">1.27.3</a> (2020-08-04)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/51e0d8b3fbc1faebf67f6dbaced1095534d7017f"><code>51e0d8b</code></a> chore(release): 1.28.1</li>
<li><a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b"><code>08e1bc5</code></a> fix: defer AES CBC w/ HMAC decryption after tag verification passes</li>
<li><a href="https://github.com/panva/jose/commit/9a8404a7592c3d56093a3bf31a4ab263721ed644"><code>9a8404a</code></a> chore(release): 1.28.0</li>
<li><a href="https://github.com/panva/jose/commit/eb482a8ab825bb54dc0a89d55b1ffc7bf6bd24f4"><code>eb482a8</code></a> style: lib/jwe/encrypt.js</li>
<li><a href="https://github.com/panva/jose/commit/e0a2d579269a4787ba997bfac9b58d641ff9fa04"><code>e0a2d57</code></a> refactor: sign.js PROCESS_RECIPIENT</li>
<li><a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13"><code>ce6836a</code></a> feat: support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>)</li>
<li><a href="https://github.com/panva/jose/commit/db6254e575e6fbc0a564b80ed9e488628187a25e"><code>db6254e</code></a> ci: improve CI runtime</li>
<li><a href="https://github.com/panva/jose/commit/1a4a68fb9a2ab5e2b796545482a4d8f1a5e6e6b7"><code>1a4a68f</code></a> chore(release): 1.27.3</li>
<li><a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4"><code>d56ec9f</code></a> fix: ensure &quot;b64&quot; is the same for all recipients edge cases</li>
<li><a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469"><code>1695423</code></a> fix: do not mutate unencoded payload when signing for multiple parties</li>
<li>Additional commits viewable in <a href="https://github.com/panva/jose/compare/v1.27.2...v1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=1.27.2&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-04-19 15:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-plugin-consortium-manual
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Depends on #849

Bumps [jose](https://github.com/panva/jose) from 1.27.2 to 1.28.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v1.28.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>), fixes <a href="https://github.com/panva/jose/security/advisories/GHSA-58f5-hfqc-jgch">CVE-2021-29443</a></li>
</ul>
<h2>v1.28.0</h2>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2>v1.27.3</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/v1.28.1/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/panva/jose/compare/v1.28.0...v1.28.1">1.28.1</a> (2021-04-09)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>defer AES CBC w/ HMAC decryption after tag verification passes (<a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b">08e1bc5</a>)</li>
</ul>
<h1><a href="https://github.com/panva/jose/compare/v1.27.3...v1.28.0">1.28.0</a> (2020-08-10)</h1>
<h3>Features</h3>
<ul>
<li>support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>) (<a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13">ce6836a</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v1.27.2...v1.27.3">1.27.3</a> (2020-08-04)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>do not mutate unencoded payload when signing for multiple parties (<a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469">1695423</a>), closes <a href="https://github-redirect.dependabot.com/panva/jose/issues/89">#89</a></li>
<li>ensure &quot;b64&quot; is the same for all recipients edge cases (<a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4">d56ec9f</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/51e0d8b3fbc1faebf67f6dbaced1095534d7017f"><code>51e0d8b</code></a> chore(release): 1.28.1</li>
<li><a href="https://github.com/panva/jose/commit/08e1bc5ce7120eac78377577acba2f811c3a0b2b"><code>08e1bc5</code></a> fix: defer AES CBC w/ HMAC decryption after tag verification passes</li>
<li><a href="https://github.com/panva/jose/commit/9a8404a7592c3d56093a3bf31a4ab263721ed644"><code>9a8404a</code></a> chore(release): 1.28.0</li>
<li><a href="https://github.com/panva/jose/commit/eb482a8ab825bb54dc0a89d55b1ffc7bf6bd24f4"><code>eb482a8</code></a> style: lib/jwe/encrypt.js</li>
<li><a href="https://github.com/panva/jose/commit/e0a2d579269a4787ba997bfac9b58d641ff9fa04"><code>e0a2d57</code></a> refactor: sign.js PROCESS_RECIPIENT</li>
<li><a href="https://github.com/panva/jose/commit/ce6836af88c9e73c29560233f15ed1760c7dcc13"><code>ce6836a</code></a> feat: support for validating issuer from a list of values (<a href="https://github-redirect.dependabot.com/panva/jose/issues/91">#91</a>)</li>
<li><a href="https://github.com/panva/jose/commit/db6254e575e6fbc0a564b80ed9e488628187a25e"><code>db6254e</code></a> ci: improve CI runtime</li>
<li><a href="https://github.com/panva/jose/commit/1a4a68fb9a2ab5e2b796545482a4d8f1a5e6e6b7"><code>1a4a68f</code></a> chore(release): 1.27.3</li>
<li><a href="https://github.com/panva/jose/commit/d56ec9f5ddc2612e5ff21fe35d45a56e7153e0e4"><code>d56ec9f</code></a> fix: ensure &quot;b64&quot; is the same for all recipients edge cases</li>
<li><a href="https://github.com/panva/jose/commit/169542363f884e4028db9f80086d631e626eb469"><code>1695423</code></a> fix: do not mutate unencoded payload when signing for multiple parties</li>
<li>Additional commits viewable in <a href="https://github.com/panva/jose/compare/v1.27.2...v1.28.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=1.27.2&new-version=1.28.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-04-19 15:00:58 +0000 UTC
    </div>
</div>

