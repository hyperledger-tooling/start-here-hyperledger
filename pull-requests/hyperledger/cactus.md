---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus

You can clone this repo on <span class="fs-3">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#822](https://api.github.com/repos/hyperledger/cactus/pulls/822)
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-test-cmd-api-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                dependencies{: .label-grey }
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

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#821](https://api.github.com/repos/hyperledger/cactus/pulls/821)
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-test-plugin-consortium-manual
                </b>
            </td>
        </tr>
        <tr>
            <td>
                dependencies{: .label-grey }
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

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#820](https://api.github.com/repos/hyperledger/cactus/pulls/820)
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.28.0 to 1.28.1 in /examples/cactus-example-supply-chain-backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                dependencies{: .label-grey }
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

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#819](https://api.github.com/repos/hyperledger/cactus/pulls/819)
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-cmd-api-server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                dependencies{: .label-grey }
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

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#818](https://api.github.com/repos/hyperledger/cactus/pulls/818)
            </td>
            <td>
                <b>
                    chore(deps): bump jose from 1.27.2 to 1.28.1 in /packages/cactus-plugin-consortium-manual
                </b>
            </td>
        </tr>
        <tr>
            <td>
                dependencies{: .label-grey }
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

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#816](https://api.github.com/repos/hyperledger/cactus/pulls/816)
            </td>
            <td>
                <b>
                    docs(whitepaper): add use-cases of car-trade, electricity-trade, and supply-chain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related with Issue #817

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 10:02:30 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#815](https://api.github.com/repos/hyperledger/cactus/pulls/815)
            </td>
            <td>
                <b>
                    chore(release): publish v1.0.0-rc.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 04:04:14 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#814](https://api.github.com/repos/hyperledger/cactus/pulls/814)
            </td>
            <td>
                <b>
                    feat(cmd-api-server): container image definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                API_Server{: .label-grey }dependencies{: .label-grey }documentation{: .label-grey }
            </td>
            <td>
                Tagged in DockerHub as a temporary measure (later will push to the
official Hyperledger Cactus repo as well):
petermetz/cactus-cmd-api-server:2021-04-18-fix-quorum-contract-types

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 03:12:02 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#813](https://api.github.com/repos/hyperledger/cactus/pulls/813)
            </td>
            <td>
                <b>
                    feat(tools): add test-npm-registry container image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                Developer_Experience{: .label-grey }dependencies{: .label-grey }
            </td>
            <td>
                ## Dependencies

#810 

## Commit to review

This is also tagged on DockerHub as
petermetz/cactus-test-npm-registry:1.0.0

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-18 21:57:46 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#812](https://api.github.com/repos/hyperledger/cactus/pulls/812)
            </td>
            <td>
                <b>
                    feat(core-api): hasTransactionFinality() on connector API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding function hasTransactionFinality() on connector API, to let ledger query whether the configured consensus has transaction finality at run time.
Fixes #354 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-18 13:31:27 +0000 UTC
    </div>
</div>

