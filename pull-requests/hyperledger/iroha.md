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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4583" class=".btn">#4583</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.1.0 to 25.2.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.1.0 to 25.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.2.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.2.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.1.0...v25.2.0">v25.2.0 - 2024-05-13</a></h3>
<ul>
<li>Update VAT generation in <code>nl_BE</code> to align with correct Belgian format. Thanks <a href="https://github.com/JorisSpruyt"><code>@​JorisSpruyt</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/db5a5ca9ef1dc9450a2a309945a7faa75007febb"><code>db5a5ca</code></a> Bump version: 25.1.0 → 25.2.0</li>
<li><a href="https://github.com/joke2k/faker/commit/aad9c23c9229ece55363c278f7b1f986b7ffc493"><code>aad9c23</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/0479fbdfb1db8002e496bd6d6aa2817b85415d1e"><code>0479fbd</code></a> :lipstick: format code</li>
<li><a href="https://github.com/joke2k/faker/commit/64ce2c6ca69412ef7d65aefa1ee788f7b3058a89"><code>64ce2c6</code></a> Update VAT generation in <code>nl_BE</code> to align with correct Belgian format (<a href="https://redirect.github.com/joke2k/faker/issues/2038">#2038</a>)</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.1.0...v25.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.1.0&new-version=25.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-13 16:16:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4582" class=".btn">#4582</a>
            </td>
            <td>
                <b>
                    chore(deps): bump parity-scale-codec from 3.6.9 to 3.6.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [parity-scale-codec](https://github.com/paritytech/parity-scale-codec) from 3.6.9 to 3.6.12.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/paritytech/parity-scale-codec/commit/57925fc782ed76d42730c83255a0d1cafef9e086"><code>57925fc</code></a> Release <code>3.6.12</code></li>
<li><a href="https://github.com/paritytech/parity-scale-codec/commit/e8b12a9dd9c530826b8ab86d620046932f5f45ac"><code>e8b12a9</code></a> Release 3.6.11 to fix a version number discrepancy between `parity-scale-code...</li>
<li><a href="https://github.com/paritytech/parity-scale-codec/commit/54462566d90a885e1e2ca8b36b3f73384b251bc4"><code>5446256</code></a> Bump parity-scale-codec version</li>
<li><a href="https://github.com/paritytech/parity-scale-codec/commit/5bf39a12719ab5b0fe151a5e823f1a91b0b554c7"><code>5bf39a1</code></a> Bump <code>proc-macro-crate</code> to v3.1.0 in 3.6.x branch (<a href="https://redirect.github.com/paritytech/parity-scale-codec/issues/590">#590</a>)</li>
<li><a href="https://github.com/paritytech/parity-scale-codec/commit/67efb534024aba892ccf38fbc753cef177bb7040"><code>67efb53</code></a> chore(docs): Restore missing doc for codec-<code>crate</code> attribute (<a href="https://redirect.github.com/paritytech/parity-scale-codec/issues/576">#576</a>)</li>
<li>See full diff in <a href="https://github.com/paritytech/parity-scale-codec/compare/v3.6.9...v3.6.12">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=parity-scale-codec&package-manager=cargo&previous-version=3.6.9&new-version=3.6.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-13 16:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4581" class=".btn">#4581</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pylint from 3.1.0 to 3.1.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pylint](https://github.com/pylint-dev/pylint) from 3.1.0 to 3.1.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pylint-dev/pylint/commit/94eed8181960ec1012eb4f4c314db3e226749f23"><code>94eed81</code></a> Bump pylint to 3.1.1, update changelog (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9615">#9615</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/461831f107ba2d4cca4d72cc76c3ad32b3c6b850"><code>461831f</code></a> Fix a false positive with <code>singledispatchmethod-function</code> (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9599">#9599</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9605">#9605</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/cf102ffb1ef4a3b1de839f86f4f4a38c685b5ebc"><code>cf102ff</code></a> Fix a false positive for <code>consider-using-dict-items</code> (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9594">#9594</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9597">#9597</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/b8b9abd5ec5990af88c2315d7d6a1afaaac6b699"><code>b8b9abd</code></a> Recognize new-style attrs decorators in too-few-public-methods check (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9346">#9346</a>) ...</li>
<li>See full diff in <a href="https://github.com/pylint-dev/pylint/compare/v3.1.0...v3.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pylint&package-manager=pip&previous-version=3.1.0&new-version=3.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-13 16:15:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4580" class=".btn">#4580</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_json from 1.0.116 to 1.0.117
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.116 to 1.0.117.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.117</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/serde-rs/json/issues/1130">#1130</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/0ae247ca63be75e6c7e6e0e9cd8916e618cf8f24"><code>0ae247c</code></a> Release 1.0.117</li>
<li><a href="https://github.com/serde-rs/json/commit/4517c7a2d983a56aa403c651cabe2caf41136570"><code>4517c7a</code></a> PartialEq is not implemented between Value and 128-bit ints</li>
<li><a href="https://github.com/serde-rs/json/commit/fdf99c7c38c1ee48554eaea66b701f470544d037"><code>fdf99c7</code></a> Combine number PartialEq tests</li>
<li><a href="https://github.com/serde-rs/json/commit/b4fc2451d726303091586758676de7ec189a315a"><code>b4fc245</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1130">#1130</a> from serde-rs/checkcfg</li>
<li><a href="https://github.com/serde-rs/json/commit/98f1a247de77176f605c39e225f81c6e80d93727"><code>98f1a24</code></a> Resolve unexpected_cfgs warning</li>
<li>See full diff in <a href="https://github.com/serde-rs/json/compare/v1.0.116...v1.0.117">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.116&new-version=1.0.117)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-13 16:15:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4579" class=".btn">#4579</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.60 to 2.0.63
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.60 to 2.0.63.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.63</h2>
<ul>
<li>Parse and print long if-else-if chains without reliance on deep recursion to avoid overflowing stack (<a href="https://redirect.github.com/dtolnay/syn/issues/1644">#1644</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1645">#1645</a>)</li>
</ul>
<h2>2.0.62</h2>
<ul>
<li>Reject invalid unparenthesized range and comparison operator expressions (<a href="https://redirect.github.com/dtolnay/syn/issues/1642">#1642</a>, <a href="https://redirect.github.com/dtolnay/syn/issues/1643">#1643</a>)</li>
</ul>
<h2>2.0.61</h2>
<ul>
<li>Check for legal binding name in the ident of Pat::Ident (<a href="https://redirect.github.com/dtolnay/syn/issues/1627">#1627</a>)</li>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/dtolnay/syn/issues/1635">#1635</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/8bcd277e4c277a8a64542287e9dd232bc27c3328"><code>8bcd277</code></a> Release 2.0.63</li>
<li><a href="https://github.com/dtolnay/syn/commit/6d1113df339f6e6fc87d16e56e3e0c5626a37a19"><code>6d1113d</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1645">#1645</a> from dtolnay/ifelse</li>
<li><a href="https://github.com/dtolnay/syn/commit/40950ddb27ff5fcfdf64dc9a4fa9fc98fd98d267"><code>40950dd</code></a> Remove recursion from printing of Expr::If</li>
<li><a href="https://github.com/dtolnay/syn/commit/e2e7f2dd2261e35c5e3f3f41296995471516531a"><code>e2e7f2d</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1644">#1644</a> from dtolnay/ifelse</li>
<li><a href="https://github.com/dtolnay/syn/commit/70777ceec1b085527392d64ebf3d9f43803187ae"><code>70777ce</code></a> Remove recursion from parsing of Expr::If</li>
<li><a href="https://github.com/dtolnay/syn/commit/e9e6329cf8b388b5323c3f2c926561687d38927e"><code>e9e6329</code></a> Release 2.0.62</li>
<li><a href="https://github.com/dtolnay/syn/commit/c79cea17721eaeec2d7ef6c9624993de9613ea26"><code>c79cea1</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1643">#1643</a> from dtolnay/chainedcompare</li>
<li><a href="https://github.com/dtolnay/syn/commit/dc4ffde94ecac024785fd4fe75e7318fbc46be22"><code>dc4ffde</code></a> Require parens for chained comparison binops</li>
<li><a href="https://github.com/dtolnay/syn/commit/c463a74f7bd4f8cd81a57c8a77faece2d2590a42"><code>c463a74</code></a> Add tests of binop associativity</li>
<li><a href="https://github.com/dtolnay/syn/commit/da509d51edddf790154133ed2a57f1fcc7387c88"><code>da509d5</code></a> Add test of assignment and range precedence</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.60...2.0.63">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.60&new-version=2.0.63)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-13 16:15:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4578" class=".btn">#4578</a>
            </td>
            <td>
                <b>
                    chore(deps): bump thiserror from 1.0.59 to 1.0.60
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [thiserror](https://github.com/dtolnay/thiserror) from 1.0.59 to 1.0.60.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/thiserror/releases">thiserror's releases</a>.</em></p>
<blockquote>
<h2>1.0.60</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/dtolnay/thiserror/issues/298">#298</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/thiserror/commit/870d11b830e7f1ce0ad6c1656806a7fcdd4273df"><code>870d11b</code></a> Release 1.0.60</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/0ccee7c2a1741d4e9a1973475cd54277891a1d92"><code>0ccee7c</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/thiserror/issues/298">#298</a> from dtolnay/checkcfg</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/cf43d0c1302f1ee073a7062b2dc24123589a4417"><code>cf43d0c</code></a> Resolve unexpected_cfgs warning</li>
<li>See full diff in <a href="https://github.com/dtolnay/thiserror/compare/1.0.59...1.0.60">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=thiserror&package-manager=cargo&previous-version=1.0.59&new-version=1.0.60)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-13 16:14:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4577" class=".btn">#4577</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.200 to 1.0.201
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.200 to 1.0.201.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.201</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/serde-rs/serde/issues/2737">#2737</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/b4f1bc16ffe9650750695db59bcb786033a929be"><code>b4f1bc1</code></a> Release 1.0.201</li>
<li><a href="https://github.com/serde-rs/serde/commit/029ab46f7185b2dcf9ec986a87142bb7e7fc97a4"><code>029ab46</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2737">#2737</a> from dtolnay/checkcfg</li>
<li><a href="https://github.com/serde-rs/serde/commit/220ca0ca9dddba8cc19d19968af7988ca3fc7d7c"><code>220ca0c</code></a> Resolve unexpected_cfgs warning</li>
<li><a href="https://github.com/serde-rs/serde/commit/20306f493a4c943459e7492caf4dbcfca717790d"><code>20306f4</code></a> Fix cfg on test_systemtime_overflow</li>
<li>See full diff in <a href="https://github.com/serde-rs/serde/compare/v1.0.200...v1.0.201">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.200&new-version=1.0.201)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-13 16:14:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4574" class=".btn">#4574</a>
            </td>
            <td>
                <b>
                    chore(deps): bump trybuild from 1.0.91 to 1.0.95
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [trybuild](https://github.com/dtolnay/trybuild) from 1.0.91 to 1.0.95.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/trybuild/releases">trybuild's releases</a>.</em></p>
<blockquote>
<h2>1.0.95</h2>
<ul>
<li>Keep long type names in diagnostics so that test output does not vary depending on the length of the absolute filepath of the crate (<a href="https://redirect.github.com/dtolnay/trybuild/issues/269">#269</a>)</li>
</ul>
<h2>1.0.94</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/dtolnay/trybuild/issues/268">#268</a>)</li>
</ul>
<h2>1.0.93</h2>
<ul>
<li>Remove dependency on <code>once_cell</code> crate (<a href="https://redirect.github.com/dtolnay/trybuild/issues/266">#266</a>, thanks <a href="https://github.com/taiki-e"><code>@​taiki-e</code></a>)</li>
</ul>
<h2>1.0.92</h2>
<ul>
<li>Update normalization of verbose type paths to accommodate error message changes in rust 1.78 (<a href="https://redirect.github.com/dtolnay/trybuild/issues/265">#265</a>, thanks <a href="https://github.com/weiznich"><code>@​weiznich</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/trybuild/commit/02e6117084d81540ff533da81a3bdd74e00cdf27"><code>02e6117</code></a> Release 1.0.95</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/619bfcd491cbdcc443e54f66aa329dc207cc6034"><code>619bfcd</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/270">#270</a> from dtolnay/typename</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/db3c9b4f545d8e9250e2defeb724d6f46c4f22cc"><code>db3c9b4</code></a> Disable long typename shortening in diagnostics</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/9ed763b56f204ecc2624657016c12aeae3d26920"><code>9ed763b</code></a> Release 1.0.94</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/b3c948124251872bc3111d2cf2938ae044e9e9d1"><code>b3c9481</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/268">#268</a> from dtolnay/checkcfg</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/7bb6f2fb22f39744771fa229740d8e023c67e424"><code>7bb6f2f</code></a> Resolve unexpected_cfgs warning</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/8a57d8c2eb84241a5986f11cb99621d8a59ce65e"><code>8a57d8c</code></a> Release 1.0.93</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/b9888357069e2cbc24a752ad5c7c125f60d178ac"><code>b988835</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/267">#267</a> from dtolnay/constmutex</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/95f8cdbd329c1c46d1a413faf3622053838eaa4d"><code>95f8cdb</code></a> Remove OnceLock around intra-process lock's mutex</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/62b1543732bb61ac0cba28d90cc5b17826ebe780"><code>62b1543</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/266">#266</a> from taiki-e/once_cell</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/trybuild/compare/1.0.91...1.0.95">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=trybuild&package-manager=cargo&previous-version=1.0.91&new-version=1.0.95)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-10 16:31:55 +0000 UTC
    </div>
</div>

