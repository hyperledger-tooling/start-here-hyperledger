---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Bump class-validator from 0.13.2 to 0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [class-validator](https://github.com/typestack/class-validator) from 0.13.2 to 0.14.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/typestack/class-validator/blob/develop/CHANGELOG.md">class-validator's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/typestack/class-validator/compare/v0.13.2...v0.14.0">0.14.0</a> (2022-12-09)</h3>
<h3>Added</h3>
<ul>
<li>add <code>@IsTimeZone</code> decorator to check if given string is valid IANA time zone</li>
<li>add <code>@IsISO4217CurrencyCode</code> decorator to check if the string is an ISO 4217 currency code</li>
<li>add <code>@IsStrongPassword</code> decorator to check if given password matches specific complexity criteria</li>
<li>add <code>@IsBase58</code> decorator to check if a string is base58 encoded</li>
<li>add <code>@IsTaxId</code> decorator to check if a given string is a valid tax ID in a given locale</li>
<li>add support for passing function as date generator in <code>@MinDate</code> and <code>@MaxDate</code> decorators</li>
<li>add option to print constraint error message instead of constraint type in validation error</li>
<li>improve decorator metadata lookup performance</li>
<li>return possible values in error message for <code>@IsEnum</code> decorator</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>re-added <code>@types/validator</code> as dependency</li>
<li>fix error generation when using <code>@NestedValidation</code></li>
<li>pass validation options correctly to validator in <code>@IsDateString</code> decorator</li>
<li>support passing <code>Symbol</code> as parameter in error message generation</li>
<li>specify supported locales for <code>@IsAlphanumeric</code> decorator</li>
<li>correctly assign decorator name in metadata instead of loosing it</li>
<li>fix various spelling errors in documentation</li>
<li>fix various spelling errors and inconsistencies in JSDoc for decorators</li>
</ul>
<h3>Changed</h3>
<ul>
<li>enable <code>forbidUnknownValues</code> option by default</li>
<li>remove documentation about deprecated schema based validation and added warning</li>
<li>update warning message logged about missing decorator metadata</li>
<li>update <code>libphonenumber-js</code> to <code>^1.10.14</code> from <code>^1.9.43</code></li>
<li>update various dev-dependencies</li>
</ul>
<h3>BREAKING CHANGES</h3>
<p><strong><code>forbidUnknownValues</code> option is enabled by default</strong></p>
<p>From this release the <code>forbidUnknownValues</code> is enabled by default. This is the desired behavior for majority of
use-cases, but this change may break validation for some. The two scenarios that results in failed validation:</p>
<ul>
<li>when attempting to validate a class instance without metadata for it</li>
<li>when using group validation and the specified validation group results in zero validation applied</li>
</ul>
<p>The old behavior can be restored via specifying <code>forbidUnknownValues: false</code> option when calling the validate functions.</p>
<p>For more details see [PR <a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1798">#1798</a>](<a href="https://github-redirect.dependabot.com/typestack/class-validator/pull/1798">typestack/class-validator#1798</a>) and <a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1422#issuecomment-1317953863">#1422 (comment)</a>.</p>
<p><strong><code>@NestedValidation</code> decorator correctly assigns validation errors</strong></p>
<p>Until now the errors from a nested validation in some cases were incorrectly assigned</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/typestack/class-validator/commit/5f0d424c164672ec981e24d6e634354803abf25f"><code>5f0d424</code></a> merge: release 0.14.0 (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1841">#1841</a>)</li>
<li><a href="https://github.com/typestack/class-validator/commit/e3d070836556b73d8396c34a360c4744c9d8363c"><code>e3d0708</code></a> build: bump version to 0.14.0</li>
<li><a href="https://github.com/typestack/class-validator/commit/ad7689055d0b92da9d6f4787cd91ec4d5392a9f1"><code>ad76890</code></a> docs: add changelog for 0.14.0</li>
<li><a href="https://github.com/typestack/class-validator/commit/9a775c59247f00f2ad911686d335fd8e1f9864be"><code>9a775c5</code></a> build(deps-dev): bump <code>@​types/node</code> from 18.11.11 to 18.11.12 (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1840">#1840</a>)</li>
<li><a href="https://github.com/typestack/class-validator/commit/53bc9f6fcefea77f17cb8e900178f25ec18b6cbc"><code>53bc9f6</code></a> build(deps-dev): bump <code>@​typescript-eslint/eslint-plugin</code> (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1837">#1837</a>)</li>
<li><a href="https://github.com/typestack/class-validator/commit/d9b40721b8911be84ae0a9e40962c6244149c7f4"><code>d9b4072</code></a> build(deps-dev): bump <code>@​typescript-eslint/parser</code> from 5.45.1 to 5.46.0 (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1838">#1838</a>)</li>
<li><a href="https://github.com/typestack/class-validator/commit/f993e9e44eb6a8cedc8ac076cee9b71760d1829d"><code>f993e9e</code></a> build(deps-dev): bump typescript from 4.9.3 to 4.9.4 (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1835">#1835</a>)</li>
<li><a href="https://github.com/typestack/class-validator/commit/ad1a41d39dee051c3a43bbd357ee0c1553b54055"><code>ad1a41d</code></a> build(deps-dev): bump <code>@​rollup/plugin-commonjs</code> from 23.0.3 to 23.0.4 (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1836">#1836</a>)</li>
<li><a href="https://github.com/typestack/class-validator/commit/42b4f7f5a34c118db14c03b6466afb5427678718"><code>42b4f7f</code></a> build(deps-dev): bump prettier from 2.8.0 to 2.8.1 (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1834">#1834</a>)</li>
<li><a href="https://github.com/typestack/class-validator/commit/0c986d4e74c498876c728c58e1b30169dccec496"><code>0c986d4</code></a> build(deps-dev): bump <code>@​types/node</code> from 18.11.10 to 18.11.11 (<a href="https://github-redirect.dependabot.com/typestack/class-validator/issues/1833">#1833</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/typestack/class-validator/compare/v0.13.2...v0.14.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=class-validator&package-manager=npm_and_yarn&previous-version=0.13.2&new-version=0.14.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 23:21:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Change ERC721 samples to use auto-indexing mint by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With this change, the default "out of the box" sample for ERC721 will _not_ require (or allow) you to pass a token index when minting. It will choose an increasing token index starting from 0.

Via ERC165 support, the connector can now check for 3 different versions of the ERC721WithData interface:
- the current version (V2), which uses auto-indexing on mint and also supports all withData/withURI methods
- the previous version (V1b), which requires explicit indexes, but supports all withData/withURI methods
- the original version (V1a), which requires explicit indexes, and supports withData but not withURI

For the "no data" variant, we have no ERC165 support, so I have destructively replaced the ERC721NoData sample with a new one that uses auto-indexing. Note that it was _just_ replaced in #104 and released as v1.2.0 - I don't really see any need to preserve all the versions of this sample, so I'm just preserving this new one and the original (not the interim one introduced in v1.2.0). This new PR will probably need to become release v1.2.1, and we'll just want to note that the sample in v1.2.0 is not supported.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 17:17:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Update README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add more details on the different smart contract variants supported, and clarify extensions on top of the base fftokens protocol.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 16:25:46 +0000 UTC
    </div>
</div>

