---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4645" class=".btn">#4645</a>
            </td>
            <td>
                <b>
                    feat: Custom instructions in executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Added ISI for custom instructions, and two tests demonstrating possible use:
* Test with one custom instruction `MintAssetForAllAccounts`
* Test with simple expression system

### Linked issue

Closes #4599

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-24 19:42:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4644" class=".btn">#4644</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.65 to 2.0.66
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.65 to 2.0.66.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.66</h2>
<ul>
<li>Allow braced structs when parsing ExprLet (<a href="https://redirect.github.com/dtolnay/syn/issues/1671">#1671</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/b992916bdac459d279bb15098507d43b1febc50e"><code>b992916</code></a> Release 2.0.66</li>
<li><a href="https://github.com/dtolnay/syn/commit/4f0a23f7e147e801a996975662b0d6e6d8a7d13b"><code>4f0a23f</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1671">#1671</a> from dtolnay/exprlet</li>
<li><a href="https://github.com/dtolnay/syn/commit/c6d87a7aa0fda4a8ef867e833d14d105d07ca62b"><code>c6d87a7</code></a> Allow braced structs when parsing ExprLet</li>
<li><a href="https://github.com/dtolnay/syn/commit/747f42f235f8e1b5551a6aeca1d2779dce413408"><code>747f42f</code></a> Update with proc-macro2 1.0.83's syntax tree sizes</li>
<li>See full diff in <a href="https://github.com/dtolnay/syn/compare/2.0.65...2.0.66">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.65&new-version=2.0.66)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-24 16:13:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4642" class=".btn">#4642</a>
            </td>
            <td>
                <b>
                    refactor(executor): remove `Visit` bound from `Validate`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4237.

<!-- Link if e.g. JIRA issue or  from another repository -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 13:50:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4640" class=".btn">#4640</a>
            </td>
            <td>
                <b>
                    refactor: remove association between domains and triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Remove the association between domains and triggers.

### Linked issue

Closes #4630.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 08:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4639" class=".btn">#4639</a>
            </td>
            <td>
                <b>
                    fix(sumeragi): Use proper view_change_index on init block load
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport of #4612

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 13:45:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4638" class=".btn">#4638</a>
            </td>
            <td>
                <b>
                    feat!: Add traits for iterable and non-iterable queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

This PR is a first step towards more type-safe queries (#4569). It adds traits for singular and iterable queries and prohibits supplying filters, sorting, pagination and batching parameters in compile time (it is already a runtime error to do so).

### Linked issue

Partially addresses #4569

### Benefits

- less error prone API
- lays foundation to allow type-checking query filters

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 12:46:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4636" class=".btn">#4636</a>
            </td>
            <td>
                <b>
                    feat: add get_original_transaction_by_hash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Added a method to retrieve a pending partially signed transaction by its transaction hash from the queue. Previously, existing methods required the entire transaction payload, which was cumbersome for other users who needed to build the entire transaction for signing. Now, only the transaction hash is needed.

### Benefits

This improvement simplifies the process for users who need to sign transactions, as they no longer need to reconstruct the entire transaction payload. Instead, they can simply use the transaction hash. This change aligns more closely with real-world use cases, making the signing process more practical and efficient.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 07:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4635" class=".btn">#4635</a>
            </td>
            <td>
                <b>
                    refactor: rename `PermissionToken` to `Permission`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Just a huge rename refactor, according to https://github.com/hyperledger/iroha/pull/4597#discussion_r1607746197. This should significantly reduce the noise of #4597 itself.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 23:51:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4634" class=".btn">#4634</a>
            </td>
            <td>
                <b>
                    docs: update the contributing guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

Updated the contributing guide with reference to issues #4502, #4501, #4433.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4585 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [X] I've read `CONTRIBUTING.md`
- [X] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 19:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4632" class=".btn">#4632</a>
            </td>
            <td>
                <b>
                    refactor(executor): Check custom visit functions in `#[derive(Visit)]`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

While working on #4599, I noticed that in custom executor it is possible to derive `Visit` with invalid `#[visit(custom())]` functions which will be ignored (only rustc error that function is unused). This PR adds check for custom visit function names to avoid potential bugs. Also I updated documentation of some proc-macros related to custom executor.

```rust
#[derive(Constructor, ValidateEntrypoints, Validate, Visit)]
#[visit(custom(visit_register_domain2))]  // typo in visit_register_domain
struct Executor {
    verdict: Result,
    block_height: u64,
}
fn visit_register_domain(...) { ... }
```

### Linked issue

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 16:30:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4629" class=".btn">#4629</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.64 to 2.0.65
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.64 to 2.0.65.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.65</h2>
<ul>
<li>Optimize the implementation of <code>Fold</code> to compile faster (<a href="https://redirect.github.com/dtolnay/syn/issues/1666">#1666</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1667">#1667</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1668">#1668</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/9f2371eefa6f681b53e4d74458d86dd41673227f"><code>9f2371e</code></a> Release 2.0.65</li>
<li><a href="https://github.com/dtolnay/syn/commit/4cd181325f3488c47866f15966977682be610da1"><code>4cd1813</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1668">#1668</a> from dtolnay/foldhelper</li>
<li><a href="https://github.com/dtolnay/syn/commit/ed54092bcea6798ab0b5ed7aca6755f8918fc79e"><code>ed54092</code></a> Eliminate gen::helper module</li>
<li><a href="https://github.com/dtolnay/syn/commit/eacc8ab1b98b590df3ce9462510fd755cddf6762"><code>eacc8ab</code></a> Eliminate FoldHelper trait</li>
<li><a href="https://github.com/dtolnay/syn/commit/6e20bb8d7799d0f4c34c144e80b3bd1b6e9afd27"><code>6e20bb8</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1667">#1667</a> from dtolnay/punctuatedfold</li>
<li><a href="https://github.com/dtolnay/syn/commit/9d95cab6d332d08903538d5ce3d6e47c1598912e"><code>9d95cab</code></a> Optimize punctuated::fold</li>
<li><a href="https://github.com/dtolnay/syn/commit/82ffe86c2b721b9985edb6f368e7366bd202bc5b"><code>82ffe86</code></a> Move Punctuated fold helper to punctuated module</li>
<li><a href="https://github.com/dtolnay/syn/commit/3dfacc1538f655d33c5c8037b14669149bcd81cd"><code>3dfacc1</code></a> Ignore manual_map clippy lint</li>
<li><a href="https://github.com/dtolnay/syn/commit/7273aa77aa09ee2562b279a5d9495a212d9c0876"><code>7273aa7</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1666">#1666</a> from dtolnay/foldhelper</li>
<li><a href="https://github.com/dtolnay/syn/commit/8124c0eb99e11cae036d2c967f91f0c456c50368"><code>8124c0e</code></a> Generate fewer monomorphizations in Fold</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.64...2.0.65">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.64&new-version=2.0.65)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 17:04:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4628" class=".btn">#4628</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pytest from 8.2.0 to 8.2.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.2.1</h2>
<h1>pytest 8.2.1 (2024-05-19)</h1>
<h2>Improvements</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12334">#12334</a>: Support for Python 3.13 (beta1 at the time of writing).</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12120">#12120</a>: Fix [PermissionError]{.title-ref} crashes arising from directories which are not selected on the command-line.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12191">#12191</a>: Keyboard interrupts and system exits are now properly handled during the test collection.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12300">#12300</a>: Fixed handling of 'Function not implemented' error under squashfuse_ll, which is a different way to say that the mountpoint is read-only.</li>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12308">#12308</a>: Fix a regression in pytest 8.2.0 where the permissions of automatically-created <code>.pytest_cache</code> directories became <code>rwx------</code> instead of the expected <code>rwxr-xr-x</code>.</li>
</ul>
<h2>Trivial/Internal Changes</h2>
<ul>
<li><a href="https://redirect.github.com/pytest-dev/pytest/issues/12333">#12333</a>: pytest releases are now attested using the recent <a href="https://github.blog/2024-05-02-introducing-artifact-attestations-now-in-public-beta/">Artifact Attestation</a> support from GitHub, allowing users to verify the provenance of pytest's sdist and wheel artifacts.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/66ff8dffdf9eee9b3dd6686de34542c49ff80dcd"><code>66ff8df</code></a> Prepare release version 8.2.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/3ffcfd122cf4674ac45f6233d9b50be6c49abeea"><code>3ffcfd1</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12340">#12340</a> from pytest-dev/backport-12334-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0b28313b46a04de08bddc18896b3e61312a0c5b3"><code>0b28313</code></a> [8.2.x] Add Python 3.13 (beta) support</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f3dd93ad8d62eb0a260d3090f31be82aafbcff13"><code>f3dd93a</code></a> [8.2.x] Attest package provenance (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12335">#12335</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/bb5a1257b0aafe5932377fa8e9fd92ab39418ac7"><code>bb5a125</code></a> [8.2.x] Spelling (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12331">#12331</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f179bf252fe2c1d0afce64b4b4bab4449e366e84"><code>f179bf2</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12327">#12327</a> from pytest-dev/backport-12325-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/2b671b5f9208650e8e42e07782d95477cc41f42a"><code>2b671b5</code></a> [8.2.x] cacheprovider: fix <code>.pytest_cache</code> not being world-readable</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/65ab7cb96c95f83e922f21bb4a8a44eda2b79707"><code>65ab7cb</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12324">#12324</a> from pytest-dev/backport-12320-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/4d5fb7d71ccc069e2f882bee0e4253eaf484d2a9"><code>4d5fb7d</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12319">#12319</a> from pytest-dev/backport-12311-to-8.2.x</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/cbe5996cc684b00397494d9590f3179de232c3ee"><code>cbe5996</code></a> [8.2.x] changelog: document unittest 8.2 change as breaking</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.2.0&new-version=8.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 17:02:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4627" class=".btn">#4627</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pylint from 3.2.0 to 3.2.2 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pylint](https://github.com/pylint-dev/pylint) from 3.2.0 to 3.2.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pylint-dev/pylint/commit/769ffd20bbf321a6cf23f5e7221a0b8221f51482"><code>769ffd2</code></a> Bump pylint to 3.2.2, update changelog (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9658">#9658</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/98c5af9bdf31a4b5291c65d3b0d5cdbb19a7f082"><code>98c5af9</code></a> Fix false-positive with contextmanager missing cleanup (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9654">#9654</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9657">#9657</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/9a9db8fa78d9523cff0f6ff0769ed4f7a4a85701"><code>9a9db8f</code></a> Update astroid to 3.2.2 (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9655">#9655</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9656">#9656</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/9223172074c4ca2bb5bff3b2c5a40190cc527fcf"><code>9223172</code></a> Bump pylint to 3.2.1, update changelog</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/926547bbbfcedd77886ec1f73ae1463daac2fa7f"><code>926547b</code></a> [trailing-comma-tuple] Fix enabling with message control locally when disable...</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/14986757c97862e59a43f787b72a1205d7f1dbf0"><code>1498675</code></a> Fix linterstats.get_module_message_count() (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9146">#9146</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9648">#9648</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/aed496ad99caf1a08dc32bd17eea0a7bac839a1b"><code>aed496a</code></a> Fix FP for <code>possibly-used-before-assignment</code> with <code>assert_never()</code> (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9645">#9645</a>) (#...</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/9dae97544b1524c0a130435766b56c9bbd23ffe9"><code>9dae975</code></a> [Backport maintenance/3.2.x] Add <code>--prefer-stubs=y</code> option (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9646">#9646</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/a03ceae2745439bd0c907cd894dac973fbfb8efe"><code>a03ceae</code></a> Add <code>--prefer-stubs=y</code> option (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9632">#9632</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/b2ea3168a30fb269b6807fcd7d86f2ab0348f699"><code>b2ea316</code></a> [Backport maintenance/3.2.x] Don't emit incorrect-variance for type parameter...</li>
<li>Additional commits viewable in <a href="https://github.com/pylint-dev/pylint/compare/v3.2.0...v3.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pylint&package-manager=pip&previous-version=3.2.0&new-version=3.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 17:02:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4626" class=".btn">#4626</a>
            </td>
            <td>
                <b>
                    chore(deps): bump anyhow from 1.0.83 to 1.0.86
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [anyhow](https://github.com/dtolnay/anyhow) from 1.0.83 to 1.0.86.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/anyhow/releases">anyhow's releases</a>.</em></p>
<blockquote>
<h2>1.0.86</h2>
<ul>
<li>Fix parse error in <code>ensure!</code> with non-literal after minus sign (<a href="https://redirect.github.com/dtolnay/anyhow/issues/373">#373</a>)</li>
</ul>
<h2>1.0.85</h2>
<ul>
<li>Improve <code>ensure!</code> macro's rules to unblock some rustc pretty-printer improvements (<a href="https://redirect.github.com/dtolnay/anyhow/issues/368">#368</a>, <a href="https://redirect.github.com/dtolnay/anyhow/issues/371">#371</a>)</li>
</ul>
<h2>1.0.84</h2>
<ul>
<li>Disallow calling <code>ensure!</code> through a <code>Not</code> impl for a type that is not <code>bool</code> (<a href="https://redirect.github.com/dtolnay/anyhow/issues/367">#367</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/anyhow/commit/8ea1819c4c7829d0eb09e54a52806f382b8d445b"><code>8ea1819</code></a> Release 1.0.86</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/0a1b405631348f38b780255ac78c86a87536feb6"><code>0a1b405</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/anyhow/issues/373">#373</a> from dtolnay/minusneg</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/e0c74f26517944f4758da61079a16d88600d37c4"><code>e0c74f2</code></a> Ensure $:literal never matches negative literal</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/013c66e92b4ec59d2c6fa224661a85e63b28f782"><code>013c66e</code></a> Fix parse error with non-literal after minus sign</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/ca7aff727bfd95422dfed63d12a9b499684b6d7b"><code>ca7aff7</code></a> Add binary operator ensure tests</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/2737bbeb59f50651ff54ca3d879a3f5d659a98ab"><code>2737bbe</code></a> Release 1.0.85</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/82b8b343893387fdb56c2816bf156139adbaed03"><code>82b8b34</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/anyhow/issues/371">#371</a> from dtolnay/split</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/ad78d70db3da4923f4d37a4a40f7b5850ec6e52e"><code>ad78d70</code></a> Preserve more token spans in expression parser</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/5cce406efa91fc60adb5367cdda8ddd169a41709"><code>5cce406</code></a> Parse comparison operators before other binary operators</li>
<li><a href="https://github.com/dtolnay/anyhow/commit/72053946780a4abad68057ec2ec426a6fd7829f3"><code>7205394</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/anyhow/issues/369">#369</a> from dtolnay/tokensplit</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/anyhow/compare/1.0.83...1.0.86">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=anyhow&package-manager=cargo&previous-version=1.0.83&new-version=1.0.86)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 17:01:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4625" class=".btn">#4625</a>
            </td>
            <td>
                <b>
                    chore(deps): bump proc-macro2 from 1.0.82 to 1.0.83
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [proc-macro2](https://github.com/dtolnay/proc-macro2) from 1.0.82 to 1.0.83.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/proc-macro2/releases">proc-macro2's releases</a>.</em></p>
<blockquote>
<h2>1.0.83</h2>
<ul>
<li>Optimize the representation of <code>Ident</code> (<a href="https://redirect.github.com/dtolnay/proc-macro2/issues/462">#462</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/1b77aca69bb7a306a5c03421ecc58ca158acebed"><code>1b77aca</code></a> Release 1.0.83</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/728eddf8cbcc92880664afb551c8accb920ad73a"><code>728eddf</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/462">#462</a> from dtolnay/identsize</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/c56c5e69ebd7790173c2be3f0bc82f0f6da7bfd4"><code>c56c5e6</code></a> Drop irrelevant capacity field from Ident representation</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/464c2eb779d1b9a29a3bf513fc9285e90e22d4a8"><code>464c2eb</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/461">#461</a> from dtolnay/sizetest</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/6f894e73d2661f6e9dd8bc3e33b39a00ee023996"><code>6f894e7</code></a> Disable span size tests when layout is randomized</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/7b357afc78f7f5a99d416b6cfcd40be806ce8062"><code>7b357af</code></a> Add additional size tests</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/abc7dff3362d2ea0825bbe15d224db986fdac774"><code>abc7dff</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/460">#460</a> from dtolnay/docsrs</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/f8d88f3ca40985d00b6939e11483b99a74d5ee9c"><code>f8d88f3</code></a> Rely on docs.rs to define --cfg=docsrs by default</li>
<li>See full diff in <a href="https://github.com/dtolnay/proc-macro2/compare/1.0.82...1.0.83">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=proc-macro2&package-manager=cargo&previous-version=1.0.82&new-version=1.0.83)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 16:58:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4622" class=".btn">#4622</a>
            </td>
            <td>
                <b>
                    fix: don't clear events buffer on wsv clone
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

When 2 transactions follow each other and the 2nd fails the events from the 1st are not emitted

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 13:29:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4620" class=".btn">#4620</a>
            </td>
            <td>
                <b>
                    refactor: Make `SignedBlock` immutable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

As I understand, the problem is that `payload` of `SignedBlock` can be modified, which will result in invalid `SignedBlock` (inconsistent `payload` and `signatures`). Currently `payload` is modified only in tests. I made `payload` private and changed such tests to create new block instead of modifying existing one.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4224

### Benefits

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 09:42:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4619" class=".btn">#4619</a>
            </td>
            <td>
                <b>
                    fix(test_network): Set myself in trusted_peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

Fix how `myself` is updated in `trusted_peers` for `test_network`.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4613  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 09:34:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4617" class=".btn">#4617</a>
            </td>
            <td>
                <b>
                    feat: support `https` for `torii_url` (#4601)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span>
            </td>
            <td>
                Close #4601
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 03:44:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4616" class=".btn">#4616</a>
            </td>
            <td>
                <b>
                    fix(executor): Added register trigger permissions in the default executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

* Closes #4586 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-19 10:20:23 +0000 UTC
    </div>
</div>

