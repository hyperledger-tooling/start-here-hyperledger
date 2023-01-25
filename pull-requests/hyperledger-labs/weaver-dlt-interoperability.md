---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/370" class=".btn">#370</a>
            </td>
            <td>
                <b>
                    Relay Image fix, Bump SDK version and Add Sikhar as maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Constants' file containing driver error messages wasn't added to relay image; added it now.
- After Francis's PR, didn't updated SDK verison, updated it in this PR.
- Update Readme to add Sikhar as current maintainer
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-25 11:25:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    Bump bumpalo from 3.10.0 to 3.12.0 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [bumpalo](https://github.com/fitzgen/bumpalo) from 3.10.0 to 3.12.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/fitzgen/bumpalo/blob/main/CHANGELOG.md">bumpalo's changelog</a>.</em></p>
<blockquote>
<h2>3.12.0</h2>
<p>Released 2023-01-17.</p>
<h3>Added</h3>
<ul>
<li>Added the <code>bumpalo::boxed::Box::bump</code> and <code>bumpalo::collections::String::bump</code>
getters to get the underlying <code>Bump</code> that a string or box was allocated into.</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Some uses of <code>Box</code> that MIRI did not previously consider as UB are now
reported as UB, and <code>bumpalo</code>'s internals have been adjusted to avoid the new
UB.</li>
</ul>
<hr />
<h2>3.11.1</h2>
<p>Released 2022-10-18.</p>
<h3>Security</h3>
<ul>
<li>Fixed a bug where when <code>std::vec::IntoIter</code> was ported to
<code>bumpalo::collections::vec::IntoIter</code>, it didn't get its underlying <code>Bump</code>'s
lifetime threaded through. This meant that <code>rustc</code> was not checking the
borrows for <code>bumpalo::collections::IntoIter</code> and this could result in
use-after-free bugs.</li>
</ul>
<hr />
<h2>3.11.0</h2>
<p>Released 2022-08-17.</p>
<h3>Added</h3>
<ul>
<li>Added support for per-<code>Bump</code> allocation limits. These are enforced only in the
slow path when allocating new chunks in the <code>Bump</code>, not in the bump allocation
hot path, and therefore impose near zero overhead.</li>
<li>Added the <code>bumpalo::boxed::Box::into_inner</code> method.</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Updated to Rust 2021 edition.</li>
<li>The minimum supported Rust version (MSRV) is now 1.56.0.</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/fitzgen/bumpalo/commit/50ba1bdd406665bd2e6ba430e167a38ed1b13964"><code>50ba1bd</code></a> Bump to 3.12.0</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/3dd36507db87e1b86617f1da88a9bc81374e7faf"><code>3dd3650</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/190">#190</a> from mattfbacon/main</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/37be9a98e4241a9cc6e534c47778cb2f4337b83f"><code>37be9a9</code></a> Merge branch 'fitzgen:main' into main</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/3664dbb7922fa1372adf53fb8767cd0fc2115267"><code>3664dbb</code></a> Add String::bump method</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/701514f553a6feab61b99e0382f314d532f57272"><code>701514f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/189">#189</a> from mattfbacon/main</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/c6507f7a4c33811a275b357004c3904261c8908c"><code>c6507f7</code></a> Add Vec::bump method</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/b1e67b7aa188d4128343858bf86a29f1c99362c6"><code>b1e67b7</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/188">#188</a> from saethlin/field-retagging</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/d325e2c94576f6806508751f945ba5985661b721"><code>d325e2c</code></a> Use ManuallyDrop with bumpalo's Box instead of mem::forget</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/c699cd1303c441953344f354892b550df6c24aa1"><code>c699cd1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/183">#183</a> from stepancheg/allocated-bytes-no-headers</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/5805a293e8ba99f2adfd9c02ee6ad2532ad52fca"><code>5805a29</code></a> Clarify allocated_bytes does not include headers</li>
<li>Additional commits viewable in <a href="https://github.com/fitzgen/bumpalo/compare/3.10.0...3.12.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=bumpalo&package-manager=cargo&previous-version=3.10.0&new-version=3.12.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 22:13:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Restructure Asset Exchange Library and Fix ContractID APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Restructure AssetExchange lib, split the code into multiple files:
    - assetSwapContracts.go: HTLC functions: lock, claim, unlock and isLocked functions go here 
    - types.go: all constants, data structures and interface go here.
    - utility.go: all good to have utility HTLC functions go here.
    - helpers.go: all common helper functions go here.
    - idGenerator.go: functions to generate keys for different purposes go here.
- Moved common claim and unlock operations in a separate function, to reduce redundancy.
- Made contractId APIs work for fungible assets as well.
- Added Badge for Besu Asset exchange, re-ordered the badges, and added link to each badge to workflow action.

Closes #366 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 18:15:29 +0000 UTC
    </div>
</div>

