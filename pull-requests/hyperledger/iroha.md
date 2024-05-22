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
                PR <a href="https://github.com/hyperledger/iroha/pull/4633" class=".btn">#4633</a>
            </td>
            <td>
                <b>
                    chore(deps): bump libsodium-sys-stable from 1.20.7 to 1.20.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [libsodium-sys-stable](https://github.com/jedisct1/libsodium-sys-stable) from 1.20.7 to 1.20.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/2da70a0da6789374ca36d9a152b29d3ce0f992da"><code>2da70a0</code></a> Update libsodium</li>
<li>See full diff in <a href="https://github.com/jedisct1/libsodium-sys-stable/compare/1.20.7...1.20.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=libsodium-sys-stable&package-manager=cargo&previous-version=1.20.7&new-version=1.20.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-21 17:00:17 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4615" class=".btn">#4615</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.63 to 2.0.64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.63 to 2.0.64.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.64</h2>
<ul>
<li>Support using ParseBuffer across <code>catch_unwind</code> (<a href="https://redirect.github.com/dtolnay/syn/issues/1646">#1646</a>)</li>
<li>Validate that the expression in a let-else ends in brace as required by rustc (<a href="https://redirect.github.com/dtolnay/syn/issues/1648">#1648</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1649">#1649</a>)</li>
<li>Legalize invalid const generic arguments by wrapping in braces (<a href="https://redirect.github.com/dtolnay/syn/issues/1654">#1654</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1655">#1655</a>)</li>
<li>Fix some expression precedence edge cases involving <code>break</code> and <code>return</code> in loop headers (<a href="https://redirect.github.com/dtolnay/syn/issues/1656">#1656</a>)</li>
<li>Always print closure bodies with a brace when the closure has an explicit return type (<a href="https://redirect.github.com/dtolnay/syn/issues/1658">#1658</a>)</li>
<li>Automatically insert necessary parentheses in ToTokens for Expr when required by expression precedence (<a href="https://redirect.github.com/dtolnay/syn/issues/1659">#1659</a>)</li>
<li>Support struct literal syntax in match guard expressions (<a href="https://redirect.github.com/dtolnay/syn/issues/1662">#1662</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/98a62cbee4f3364787a4a04a9c18f2831ebb7e0a"><code>98a62cb</code></a> Release 2.0.64</li>
<li><a href="https://github.com/dtolnay/syn/commit/1f8eddbf4fa8b6536c4a938ed9fef17871d1e42a"><code>1f8eddb</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1662">#1662</a> from dtolnay/guardstruct</li>
<li><a href="https://github.com/dtolnay/syn/commit/0a3d3bd837905bc48c6c2082f92cb7cbb2788d0d"><code>0a3d3bd</code></a> Fix parsing of struct literal in match guard expression</li>
<li><a href="https://github.com/dtolnay/syn/commit/f4641931718f41ab0a81c173d8e4fc1f38fe772e"><code>f464193</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1659">#1659</a> from dtolnay/needspar</li>
<li><a href="https://github.com/dtolnay/syn/commit/afa1c7259aa6ef5795e922f7820d95fc205a74f9"><code>afa1c72</code></a> Add more auto-parenthesization tests</li>
<li><a href="https://github.com/dtolnay/syn/commit/532d3a37cf33ef13e5a878a9efdde2415b4cd2fe"><code>532d3a3</code></a> Insert necessary parentheses in ToTokens for Expr</li>
<li><a href="https://github.com/dtolnay/syn/commit/1b6a45079d2cfde0731ea47a23f5713f47d88d73"><code>1b6a450</code></a> Add test of parenthesis insertion by Expr's ToTokens</li>
<li><a href="https://github.com/dtolnay/syn/commit/83ea28918bcac980b7382c64ffe8982c70a01a18"><code>83ea289</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1658">#1658</a> from dtolnay/closurebrace</li>
<li><a href="https://github.com/dtolnay/syn/commit/206d897ed8dd784d7a36e7ca3b0920052c025cbc"><code>206d897</code></a> Create braces around closure body during printing if needed</li>
<li><a href="https://github.com/dtolnay/syn/commit/9b60027c1605420778f41a1082ec80fd730b0c25"><code>9b60027</code></a> Ignore struct_excessive_bools pedantic clippy lint</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.63...2.0.64">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.63&new-version=2.0.64)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-17 16:59:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4614" class=".btn">#4614</a>
            </td>
            <td>
                <b>
                    chore(deps): bump thiserror from 1.0.60 to 1.0.61
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [thiserror](https://github.com/dtolnay/thiserror) from 1.0.60 to 1.0.61.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/thiserror/releases">thiserror's releases</a>.</em></p>
<blockquote>
<h2>1.0.61</h2>
<ul>
<li>Use <code>core::fmt</code> and <code>core::panic</code> to facilitate <code>error_in_core</code> support (<a href="https://redirect.github.com/dtolnay/thiserror/issues/299">#299</a>, thanks <a href="https://github.com/jordens"><code>@​jordens</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/thiserror/commit/5c8016393fec09330ae495d71edee4d8104a9466"><code>5c80163</code></a> Release 1.0.61</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/e3b1b91ced4e590ac8823fa0945f01a0560dada9"><code>e3b1b91</code></a> Format PR 299 with rustfmt</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/6b2b871f39cfb0a24c24d9d27b145a9fd0a6a714"><code>6b2b871</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/thiserror/issues/299">#299</a> from quartiq/core</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/ce974bc2bd7773ef6e2cf19a2e35c0d31519c353"><code>ce974bc</code></a> also {std -&gt; core}::panic::UnwindSafe</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/7b6e35b992e96581ed5feee917fdb3c2d5918839"><code>7b6e35b</code></a> use core::fmt instead of std::fmt</li>
<li>See full diff in <a href="https://github.com/dtolnay/thiserror/compare/1.0.60...1.0.61">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=thiserror&package-manager=cargo&previous-version=1.0.60&new-version=1.0.61)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-17 16:59:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4612" class=".btn">#4612</a>
            </td>
            <td>
                <b>
                    fix(sumeragi): Use proper view_change_index on init block load
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

- if error  shutdown happened while iroha was listening for genesis exit happens gracefully
- loading blocks now respect fallback peer order

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4604 <!-- Replace with an actual number,  -->

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
        Created At 2024-05-17 13:45:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4611" class=".btn">#4611</a>
            </td>
            <td>
                <b>
                    fix(kura): Inline kura initialization into constructor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

Due `init` was separate functions error was introduced where `start` was called before initialization which cause panic in kura.

Fix for that is to inline `init` inside constructor.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4603 <!-- Replace with an actual number,  -->

### How to reproduce

1. start iroha
2. submit few blocks
3. restart iroha

Previously kura would crash, but iroha would continue working without ability to write new blocks to the disk.

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
        Created At 2024-05-17 09:38:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4610" class=".btn">#4610</a>
            </td>
            <td>
                <b>
                    refactor!: rename TransactionValue into CommittedTransaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

closes #4517 

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
        Created At 2024-05-17 05:47:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4609" class=".btn">#4609</a>
            </td>
            <td>
                <b>
                    [BACKPORT]: make TransactionValue::error field public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Closes #4561

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
        Created At 2024-05-17 05:39:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4608" class=".btn">#4608</a>
            </td>
            <td>
                <b>
                    chore(deps): bump proc-macro2 from 1.0.81 to 1.0.82
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [proc-macro2](https://github.com/dtolnay/proc-macro2) from 1.0.81 to 1.0.82.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/proc-macro2/releases">proc-macro2's releases</a>.</em></p>
<blockquote>
<h2>1.0.82</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/dtolnay/proc-macro2/issues/456">#456</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/8dc63f36f6735ff2e384e34422f57f393929f09f"><code>8dc63f3</code></a> Release 1.0.82</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/790cb418978e41899c286752803a77ba8a817d20"><code>790cb41</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/457">#457</a> from dtolnay/defaultfeatures</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/2ebe71180da1813be5dc3f77ce13020a49455c95"><code>2ebe711</code></a> Fix use of deprecated default_features in Cargo.toml</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/a720819a80afd67b10062d819c742d7cb05934cc"><code>a720819</code></a> Delete unused nightly cfg</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/37c5d18ec0e7b8a5c15cc3934ce136c2d2ee1220"><code>37c5d18</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/456">#456</a> from dtolnay/checkcfg</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/5e02f52b954f40a4cb8f26020c3ff494c3c5426a"><code>5e02f52</code></a> Suppress unknown_lints warning on old rustc</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/2660d3026a70e1478997c55044c76529ca157eda"><code>2660d30</code></a> Resolve unexpected_cfgs warning</li>
<li>See full diff in <a href="https://github.com/dtolnay/proc-macro2/compare/1.0.81...1.0.82">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=proc-macro2&package-manager=cargo&previous-version=1.0.81&new-version=1.0.82)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-16 16:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4607" class=".btn">#4607</a>
            </td>
            <td>
                <b>
                    chore(deps): bump darling from 0.20.8 to 0.20.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [darling](https://github.com/TedDriggs/darling) from 0.20.8 to 0.20.9.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/TedDriggs/darling/blob/master/CHANGELOG.md">darling's changelog</a>.</em></p>
<blockquote>
<h2>v0.20.9 (May 15, 2024)</h2>
<ul>
<li>Allow word-form for newtype enum variants whose only field produces a value when <code>from_none</code> is called on their type <a href="https://redirect.github.com/TedDriggs/darling/issues/249">#249</a></li>
<li>Add <code>FromMeta</code> impls for the <code>std::num::NonZero*</code> types <a href="https://redirect.github.com/TedDriggs/darling/pull/288">#288</a></li>
<li>Fix panic in number <code>FromMeta</code> impls when the parsed value is too large for the receiver type <a href="https://redirect.github.com/TedDriggs/darling/issues/289">#289</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/TedDriggs/darling/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=darling&package-manager=cargo&previous-version=0.20.8&new-version=0.20.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-16 16:26:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4606" class=".btn">#4606</a>
            </td>
            <td>
                <b>
                    refactor: Reject `BlockMessages` eagerly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Currently we may ignore `BlockMessage::BlockCreated` if it's view change index is less then view change index of control message received in same invocation of `receive_network_packet` function. E.g. currently we have such behaviour:
```
function receive_network_packet invoked
received block message with vc#1
received control message with vc#2
=> ignored block message with vc#1
```

This PR extends this behaviour to support more cases, e.g.:
```
function receive_network_packet invoked
received control message with vc#2

function receive_network_packet invoked
received block message with vc#1
=> ignored block message with vc#1
```

### Linked issue

Closes #4223

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
        Created At 2024-05-16 16:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4605" class=".btn">#4605</a>
            </td>
            <td>
                <b>
                    ci: Refactor Sonarqube & DefectDojo job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Move `workspace_analysis`, `with_coverage` and  `sonarqube-defectdojo` jobs to the new dedicated workflow.
2. Change docker registries repo for `iroha2:dev` and `iroha2-nightly` images.

### Linked issue
#4510 #4598 

### Closes
(should): #4510 #4598 

### Benefits
Fix clippy and lcov reports uploading to Sonarqube and DefectDojo.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 15:32:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4600" class=".btn">#4600</a>
            </td>
            <td>
                <b>
                    [BACKPORT]: support https URL scheme in config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

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
        Created At 2024-05-16 09:31:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4597" class=".btn">#4597</a>
            </td>
            <td>
                <b>
                    feat!: unify executor data model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                _Reopening #4596 due to some GitHub force-push branch-recreate issues_

---

## Description

This PR solves a few problems:

- Allows executor define its config parameters through a single `ExecutorDataModel` entity.
- Unifies parameters and permission tokens to `ExecutorDataModelObject` trait, having a `definition_id` and an arbitrary JSON `payload` (possible to support SCALE too):
  - #4352
  - #3901
- Parameters no longer configure Sumeragi/WASM/limits. I.e. chain wide configuration could only be set through the config file. **It is temporary:** this PR is a preparation for a proper implementation of chain-wide configuration: #4028
- Removes extra `PermissionTokenSchemaUpdated` event. Since this action only happens during executor migration, which emits its own event `ExecutorEvent::Upgraded`, I also included the updated `ExecutorDataModel` in this event.

## Linked issue

Closes #4352
Closes #3901
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 04:19:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4595" class=".btn">#4595</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pylint from 3.1.1 to 3.2.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pylint](https://github.com/pylint-dev/pylint) from 3.1.1 to 3.2.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pylint-dev/pylint/commit/b738d233e2df7651abae847e2331e2621482e5fb"><code>b738d23</code></a> Bump pylint to 3.2.0, update changelog</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/040ce17d4af578112dd892ea7445cd6b78ed71c1"><code>040ce17</code></a> Upgrade the contributors lists</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/743a04de97e566968510bcd398ac93490beb252a"><code>743a04d</code></a> [performance] Check that 'trailing-comma-tuple' is enabled only once (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9620">#9620</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/b4a9535566b149d5afe60b8e82d573441fbec0e6"><code>b4a9535</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9621">#9621</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/a4f9b8618f1d8ac2adde8a729e29d9a2018fdc7b"><code>a4f9b86</code></a> [pre-commit.ci] pre-commit autoupdate</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/4f0c7acfc8032c5f41cc0f429db83eb81bf3f570"><code>4f0c7ac</code></a> Merge maintenance/3.1.x into main following 3.1.1 release (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9618">#9618</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/0d8ef10c7999f33b033ee1bca3e3aad91ff0d835"><code>0d8ef10</code></a> Merge maintenance/3.1.x into main following 3.1.1 release</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/e53fdb6dbc97dae5e086d30b5d0fb0fa218b1915"><code>e53fdb6</code></a> Bump furo from 2024.4.27 to 2024.5.6 (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9617">#9617</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/814bf947541c198dc3bc8f38240113a78bf2b57a"><code>814bf94</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9616">#9616</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/fd6790b062039e42523f674ebff205e89e9eef51"><code>fd6790b</code></a> Add ignored modules to Astroid module deny list (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9504">#9504</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pylint-dev/pylint/compare/v3.1.1...v3.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pylint&package-manager=pip&previous-version=3.1.1&new-version=3.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-15 16:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4594" class=".btn">#4594</a>
            </td>
            <td>
                <b>
                    chore(deps): bump erased-serde from 0.4.4 to 0.4.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [erased-serde](https://github.com/dtolnay/erased-serde) from 0.4.4 to 0.4.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/erased-serde/releases">erased-serde's releases</a>.</em></p>
<blockquote>
<h2>0.4.5</h2>
<ul>
<li>Relocate some unsafe code over to <code>typeid</code> crate</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/erased-serde/commit/ea494262ade2d4794ad0a7ff7dabb0292baa1bdd"><code>ea49426</code></a> Release 0.4.5</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/52b9d2182efac04f3e4e9a34feee9d21265a8806"><code>52b9d21</code></a> Use non-static TypeId implementation from typeid crate</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/6516c7e8d7dc7683d5005b7abf8f1737fce81f6b"><code>6516c7e</code></a> Raise minimum tested compiler to 1.70</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/2dd7db385c6599b1d4f83fe317da1a731b44c43f"><code>2dd7db3</code></a> Raise required compiler to rust 1.61</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/011c74c53c943c7575b8b1ae0b13eed11bb34543"><code>011c74c</code></a> Revert &quot;Temporarily disable miri on doctests&quot;</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/070fd66e6f1b46c2aa4f8a618d556a4a0ccb6f9c"><code>070fd66</code></a> Explicitly install a Rust toolchain for cargo-outdated job</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/df741c319c701a004f405c5acaac5da3c4b3fcf7"><code>df741c3</code></a> Exclude benches from miri</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/fd1bb3d39b50c4ed377338cb300ad1d485344935"><code>fd1bb3d</code></a> Temporarily disable miri on doctests</li>
<li>See full diff in <a href="https://github.com/dtolnay/erased-serde/compare/0.4.4...0.4.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=erased-serde&package-manager=cargo&previous-version=0.4.4&new-version=0.4.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-15 16:31:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4593" class=".btn">#4593</a>
            </td>
            <td>
                <b>
                    chore(deps): bump trybuild from 1.0.95 to 1.0.96
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [trybuild](https://github.com/dtolnay/trybuild) from 1.0.95 to 1.0.96.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/trybuild/releases">trybuild's releases</a>.</em></p>
<blockquote>
<h2>1.0.96</h2>
<ul>
<li>Support Windows builds that have OUT_DIR prefixed with <code>\\?\</code> (<a href="https://redirect.github.com/dtolnay/trybuild/issues/271">#271</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/trybuild/commit/b1b7064b7ad11e0ab563e9eb843651d86e4545b7"><code>b1b7064</code></a> Release 1.0.96</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/742c6b3583159bf1d44ed2bef52710b0b7b6cfa6"><code>742c6b3</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/271">#271</a> from dtolnay/windows</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/7c8c3640f6a59ca2ed458c42b14e17df6956b00a"><code>7c8c364</code></a> Support OUT_DIR located in \?\ path on Windows</li>
<li>See full diff in <a href="https://github.com/dtolnay/trybuild/compare/1.0.95...1.0.96">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=trybuild&package-manager=cargo&previous-version=1.0.95&new-version=1.0.96)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-15 16:30:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4592" class=".btn">#4592</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.201 to 1.0.202
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.201 to 1.0.202.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.202</h2>
<ul>
<li>Provide public access to RenameAllRules in serde_derive_internals (<a href="https://redirect.github.com/serde-rs/serde/issues/2743">#2743</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/9e32a40b1c745d1d67d451cc983fab5751d394a5"><code>9e32a40</code></a> Release 1.0.202</li>
<li><a href="https://github.com/serde-rs/serde/commit/87f635e54d5359fa0eb94b1ef0a684ee3d24cb85"><code>87f635e</code></a> Release serde_derive_internals 0.29.1</li>
<li><a href="https://github.com/serde-rs/serde/commit/d4b2dfbde288e0ba5d4dc7852e1b8029208cf9b6"><code>d4b2dfb</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2743">#2743</a> from dtolnay/renameallrules</li>
<li><a href="https://github.com/serde-rs/serde/commit/f6ab0bc56f3df6d03974d233ffce352b0725ae09"><code>f6ab0bc</code></a> Provide public access to RenameAllRules in serde_derive_internals</li>
<li><a href="https://github.com/serde-rs/serde/commit/48cc2a63279d4ea44a88d566b0667f65c9ea79f4"><code>48cc2a6</code></a> Replace use of a syn From impl</li>
<li><a href="https://github.com/serde-rs/serde/commit/3202a6858a2802b5aba2fa5cf3ec8f203408db74"><code>3202a68</code></a> Skip rerunning build script on library code changes</li>
<li>See full diff in <a href="https://github.com/serde-rs/serde/compare/v1.0.201...v1.0.202">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.201&new-version=1.0.202)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-15 16:29:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4591" class=".btn">#4591</a>
            </td>
            <td>
                <b>
                    chore(deps): bump toml from 0.8.12 to 0.8.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [toml](https://github.com/toml-rs/toml) from 0.8.12 to 0.8.13.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/toml-rs/toml/commit/912761bd748d9b6fb9eedf3a8be68ab698388a78"><code>912761b</code></a> chore: Release</li>
<li><a href="https://github.com/toml-rs/toml/commit/40b02a3d5500fc1b3ab2f64c09175d780822d1a1"><code>40b02a3</code></a> Merge pull request <a href="https://redirect.github.com/toml-rs/toml/issues/730">#730</a> from epage/msrv</li>
<li><a href="https://github.com/toml-rs/toml/commit/8eb5dcb6475e6ea47d4bac80927392b3dc9a2110"><code>8eb5dcb</code></a> fix: Drop MSRV to 1.65</li>
<li><a href="https://github.com/toml-rs/toml/commit/f9249d83e5e43a605fcf214db8d779aa798ce104"><code>f9249d8</code></a> Merge pull request <a href="https://redirect.github.com/toml-rs/toml/issues/726">#726</a> from mistydemeo/fix_typo</li>
<li><a href="https://github.com/toml-rs/toml/commit/1e3e03305bbc13f5b6468b4a44921fd5ef89f104"><code>1e3e033</code></a> docs: fix typo</li>
<li><a href="https://github.com/toml-rs/toml/commit/adbc75b9716170d9f19798bfe33c16a814b3bea3"><code>adbc75b</code></a> chore(deps): Update Rust Stable to v1.78 (<a href="https://redirect.github.com/toml-rs/toml/issues/724">#724</a>)</li>
<li><a href="https://github.com/toml-rs/toml/commit/f8b1b263d425a1b1f036b13d115fdc4cbb031ac4"><code>f8b1b26</code></a> Merge pull request <a href="https://redirect.github.com/toml-rs/toml/issues/725">#725</a> from epage/update</li>
<li><a href="https://github.com/toml-rs/toml/commit/7eef906a43df1c85940c83e1cda9cefb2a010883"><code>7eef906</code></a> style: Address warnings</li>
<li><a href="https://github.com/toml-rs/toml/commit/813ce3d757bb0276267cba1a8f8e49f5bc4b0a32"><code>813ce3d</code></a> chore(deps): Update compatible (dev) (<a href="https://redirect.github.com/toml-rs/toml/issues/723">#723</a>)</li>
<li><a href="https://github.com/toml-rs/toml/commit/66f7f1a1989e0756cd03cb8347c2383df694d8d6"><code>66f7f1a</code></a> docs: Remove stale content from examples</li>
<li>Additional commits viewable in <a href="https://github.com/toml-rs/toml/compare/toml-v0.8.12...toml-v0.8.13">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=toml&package-manager=cargo&previous-version=0.8.12&new-version=0.8.13)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-15 16:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4590" class=".btn">#4590</a>
            </td>
            <td>
                <b>
                    chore(deps): bump libsodium-sys-stable from 1.20.6 to 1.20.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [libsodium-sys-stable](https://github.com/jedisct1/libsodium-sys-stable) from 1.20.6 to 1.20.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/acefb65f4b18f8b9e5b08aa8716c8acb4c3f6db3"><code>acefb65</code></a> Fetch using http</li>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/1c2dd602d15e584504bae375ebc5a0b3bb5548a8"><code>1c2dd60</code></a> Remove test on x86_64-darwin</li>
<li>See full diff in <a href="https://github.com/jedisct1/libsodium-sys-stable/compare/1.20.6...1.20.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=libsodium-sys-stable&package-manager=cargo&previous-version=1.20.6&new-version=1.20.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-15 16:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4589" class=".btn">#4589</a>
            </td>
            <td>
                <b>
                    fix: trigger set is correctly serialized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

Properly serialize trigger set.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4588 <!-- Replace with an actual number,  -->

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
        Created At 2024-05-15 10:47:49 +0000 UTC
    </div>
</div>

