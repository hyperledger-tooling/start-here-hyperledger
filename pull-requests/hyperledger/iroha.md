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
                PR <a href="https://github.com/hyperledger/iroha/pull/4792" class=".btn">#4792</a>
            </td>
            <td>
                <b>
                    fix: flatten asset definitions and assets in data model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
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
        Created At 2024-06-30 22:45:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4791" class=".btn">#4791</a>
            </td>
            <td>
                <b>
                    refactor!: split executor data model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

* remove `derive` crates from workspace dependencies
* split `executor` into `data_model` and `core` crates 
* rewrite tests/examples so that they use statically typed permissions

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

* we will never see `json!` again

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
        Created At 2024-06-30 10:27:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4790" class=".btn">#4790</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pylint from 3.2.4 to 3.2.5 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pylint](https://github.com/pylint-dev/pylint) from 3.2.4 to 3.2.5.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pylint-dev/pylint/commit/ae730ac7721d2cb206c153f680605b83d66fbc84"><code>ae730ac</code></a> Bump pylint to 3.2.5, update changelog (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9756">#9756</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/be7b5cc8cb3bf910866b66eb43becabf5299ab2f"><code>be7b5cc</code></a> [unreachable-code] Fix the false positive in python 3.8 (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9753">#9753</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9755">#9755</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/6c3ab77c23cb3c6fe4a626148bf3aab9de8f3dd6"><code>6c3ab77</code></a> [release] Fix 3.2.4 release date following issue with twine 5.1.0 (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9749">#9749</a>) (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9">#9</a>...</li>
<li>See full diff in <a href="https://github.com/pylint-dev/pylint/compare/v3.2.4...v3.2.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pylint&package-manager=pip&previous-version=3.2.4&new-version=3.2.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-28 16:31:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4789" class=".btn">#4789</a>
            </td>
            <td>
                <b>
                    chore(deps): bump log from 0.4.21 to 0.4.22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [log](https://github.com/rust-lang/log) from 0.4.21 to 0.4.22.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rust-lang/log/blob/master/CHANGELOG.md">log's changelog</a>.</em></p>
<blockquote>
<h2>[0.4.22] - 2024-06-27</h2>
<h2>What's Changed</h2>
<ul>
<li>Add some clarifications to the library docs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/620">rust-lang/log#620</a></li>
<li>Add links to <code>colog</code> crate by <a href="https://github.com/chrivers"><code>@​chrivers</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/621">rust-lang/log#621</a></li>
<li>adding line_number test + updating some testing infrastructure by <a href="https://github.com/DIvkov575"><code>@​DIvkov575</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/619">rust-lang/log#619</a></li>
<li>Clarify the actual set of functions that can race in _racy variants by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/623">rust-lang/log#623</a></li>
<li>Replace deprecated std::sync::atomic::spin_loop_hint() by <a href="https://github.com/Catamantaloedis"><code>@​Catamantaloedis</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/625">rust-lang/log#625</a></li>
<li>Check usage of max_level features by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/627">rust-lang/log#627</a></li>
<li>Remove unneeded import by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/628">rust-lang/log#628</a></li>
<li>Loosen orderings for logger initialization in <a href="https://redirect.github.com/rust-lang/log/pull/632">rust-lang/log#632</a>. Originally by <a href="https://github.com/pwoolcoc"><code>@​pwoolcoc</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/599">rust-lang/log#599</a></li>
<li>Use Location::caller() for file and line info in <a href="https://redirect.github.com/rust-lang/log/pull/633">rust-lang/log#633</a>. Originally by <a href="https://github.com/Cassy343"><code>@​Cassy343</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/520">rust-lang/log#520</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/chrivers"><code>@​chrivers</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/621">rust-lang/log#621</a></li>
<li><a href="https://github.com/DIvkov575"><code>@​DIvkov575</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/619">rust-lang/log#619</a></li>
<li><a href="https://github.com/Catamantaloedis"><code>@​Catamantaloedis</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/625">rust-lang/log#625</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/rust-lang/log/compare/0.4.21...0.4.22">https://github.com/rust-lang/log/compare/0.4.21...0.4.22</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rust-lang/log/commit/d5ba2cfee9b3b4ca1fcad911b7f59dc79eeee022"><code>d5ba2cf</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/634">#634</a> from rust-lang/cargo/0.4.22</li>
<li><a href="https://github.com/rust-lang/log/commit/d1a8306aadb88d56b74c73cdce4ef0153fb549cb"><code>d1a8306</code></a> prepare for 0.4.22 release</li>
<li><a href="https://github.com/rust-lang/log/commit/46894ef229483bbabd30a806c474417fc034559c"><code>46894ef</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/633">#633</a> from rust-lang/feat/panic-info</li>
<li><a href="https://github.com/rust-lang/log/commit/e0d389c9cadd91363f2fec52bd30f9585168a89f"><code>e0d389c</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/632">#632</a> from rust-lang/feat/loosen-atomics</li>
<li><a href="https://github.com/rust-lang/log/commit/c9e5e13e9b02ec80e784c6fe4deacdc8f3194fca"><code>c9e5e13</code></a> use Location::caller() for file and line info</li>
<li><a href="https://github.com/rust-lang/log/commit/507b672660288f0223edb6353d34f8733fa0a2f4"><code>507b672</code></a> loosen orderings for logger initialization</li>
<li><a href="https://github.com/rust-lang/log/commit/c879b011a8ac662545adf9484d9a668ebcf9b814"><code>c879b01</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/628">#628</a> from Thomasdezeeuw/fix-warnings</li>
<li><a href="https://github.com/rust-lang/log/commit/405fdb4d9f847c93c0133469ea808f09320714ba"><code>405fdb4</code></a> Merge pull request <a href="https://redirect.github.com/rust-lang/log/issues/627">#627</a> from Thomasdezeeuw/check-features</li>
<li><a href="https://github.com/rust-lang/log/commit/1307ade1122549badf2b8fdd10c11e519eaa029a"><code>1307ade</code></a> Remove unneeded import</li>
<li><a href="https://github.com/rust-lang/log/commit/710560ecb7035a6baf1fd9d97d7f09d0cc075006"><code>710560e</code></a> Don't use --all-features in CI</li>
<li>Additional commits viewable in <a href="https://github.com/rust-lang/log/compare/0.4.21...0.4.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log&package-manager=cargo&previous-version=0.4.21&new-version=0.4.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-28 16:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4788" class=".btn">#4788</a>
            </td>
            <td>
                <b>
                    feat!: reimplement multisignature transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

This PR provide an example how multisignature transactions could be implemented using iroha triggers.
In this PR i've tried to make as small invasive changes into the core as possible.

How this work?

There is 2 triggers (thanks @s8sato  for inspiration in account activation feature): 
1. `multisig_register` - responsible for registering new multisig user and trigger `multisig`
2. `multisig` - responsible for executing instructions on behalf of multisig user when enough votes are collected  

Assumptions: 
- user have to come up with they own public key for multisig account:
    - it might be ok to have primary private key in case of emergency or smt
    - it could be generated at random or obtained through key aggregation
    - it's currently not possible to generate public key inside wasm smart-contracts
- `multisig_register` should be registered either as part of genesis or by domain owner to have enough permissions for it's actions
    - currently in default executor there is no way to allow certain trigger to be executable by anyone (workaround would be to have trigger which would grant this permission on account registration)

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4373 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Get back multisig functionality without too much changes on iroha side.

### Downsides

Executing multisig instructions through tirgger probably slower that backed in solution.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2024-06-28 12:22:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4787" class=".btn">#4787</a>
            </td>
            <td>
                <b>
                    refactor(env)!: simplify naming of env variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

* rename `GENESIS_SIGNED_FILE` to `GENESIS`
* rename `SUMERAGI_TRUSTED_PEERS` to `TRUSTED_PEERS`

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
        Created At 2024-06-28 11:17:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4786" class=".btn">#4786</a>
            </td>
            <td>
                <b>
                    refactor: Add #[ignore] to the sorting test
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
        Created At 2024-06-28 08:59:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4785" class=".btn">#4785</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.9.2 to 26.0.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.9.2 to 26.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v26.0.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v26.0.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.9.2...v26.0.0">v26.0.0 - 2024-06-26</a></h3>
<ul>
<li>Fix upper limit of nb_elements. Thanks <a href="https://github.com/mileswatsonbjss"><code>@​mileswatsonbjss</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/554d1aa1ce75ff26cf36e35fa9aafb9f03d1e5f4"><code>554d1aa</code></a> Bump version: 25.9.2 → 26.0.0</li>
<li><a href="https://github.com/joke2k/faker/commit/8d31b08aa2c53b6b1da5d4ac205fe04af9af7182"><code>8d31b08</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/39feef74a8ef17b6ca08b8740dcfbfe785bb7177"><code>39feef7</code></a> issue a warning instead of logging when elements don’t match word count</li>
<li><a href="https://github.com/joke2k/faker/commit/fb8b8a2840edac237a33cdda6564e7824acd806c"><code>fb8b8a2</code></a> Rename <code>word_list</code> argument to <code>words()</code> back to <code>ext_word_list</code></li>
<li><a href="https://github.com/joke2k/faker/commit/b01507adb7df51114adfa2fbe927b328476f8b57"><code>b01507a</code></a> Fix upper limit of nb_elements (<a href="https://redirect.github.com/joke2k/faker/issues/2067">#2067</a>)</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.9.2...v26.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.9.2&new-version=26.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-27 16:52:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4778" class=".btn">#4778</a>
            </td>
            <td>
                <b>
                    refactor: improve custom instruction usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
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
        Created At 2024-06-26 18:59:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4777" class=".btn">#4777</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.9.1 to 25.9.2 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.9.1 to 25.9.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.9.2</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.9.2/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.9.1...v25.9.2">v25.9.2 - 2024-06-25</a></h3>
<ul>
<li>Remove duplicate entry in currency provider.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/97c046c70bdc208caed8c35646edab00bd7de476"><code>97c046c</code></a> Bump version: 25.9.1 → 25.9.2</li>
<li><a href="https://github.com/joke2k/faker/commit/e4949d40312cb4f7337bf4131370c5d82990eaae"><code>e4949d4</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/667d9076ba1aea60fa2ab0802407822ad217e157"><code>667d907</code></a> Remove duplicate entry in currency provider</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.9.1...v25.9.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.9.1&new-version=25.9.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-26 16:45:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4776" class=".btn">#4776</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump pylint from 3.2.3 to 3.2.4 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pylint](https://github.com/pylint-dev/pylint) from 3.2.3 to 3.2.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pylint-dev/pylint/commit/425ad66da9467bac9074de3f2294f7851cb3320b"><code>425ad66</code></a> Bump pylint to 3.2.4, update changelog (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9746">#9746</a>)</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/c41c35a8e0dd71ba96944613e6a2ced830407670"><code>c41c35a</code></a> [possibly-used-before-assignment] Avoid FP for typing.NoReturn &amp; Never (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9714">#9714</a>...</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/22e4d365277d20b243de54e7a75cedde28436b11"><code>22e4d36</code></a> [symilar] Rename the unittest file that had a typo.</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/3cf313a2abacfc273a4b26ecf94f9dc2fc61a00d"><code>3cf313a</code></a> [symilar] Fix the short form options that weren't being processed properly</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/e13544f4e2ce93e823019958e05f5e590169992d"><code>e13544f</code></a> [symilar] Fix crash when giving bad options to symilar</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/c3e257925e313a19f42dd17d20179152f5f5db2f"><code>c3e2579</code></a> [unnecessary-list-index-lookup] Fix crashes for uninferrable 'start' value in...</li>
<li><a href="https://github.com/pylint-dev/pylint/commit/6b66ca65b2c8e4562d5550694ba68bb6bb445034"><code>6b66ca6</code></a> [undefined-variable] Fix a crash for undefined lineno in annotations (<a href="https://redirect.github.com/pylint-dev/pylint/issues/9705">#9705</a>) ...</li>
<li>See full diff in <a href="https://github.com/pylint-dev/pylint/compare/v3.2.3...v3.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pylint&package-manager=pip&previous-version=3.2.3&new-version=3.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-26 16:45:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4775" class=".btn">#4775</a>
            </td>
            <td>
                <b>
                    feat: Allow multiple peers submit genesis block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Continuation of #4739:
* Topology stored in genesis block will be used as initial topology, as a result multiple peers can submit genesis
* Removed `--submit-genesis` flag
* Changed `scripts/test_env.py`, it will submit genesis for all peers

### Linked issue

Closes #4696

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
        Created At 2024-06-26 16:44:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4774" class=".btn">#4774</a>
            </td>
            <td>
                <b>
                    test: update client cli tests
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

Closes #4755 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
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
        Created At 2024-06-26 13:12:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4773" class=".btn">#4773</a>
            </td>
            <td>
                <b>
                    fix: fix apply/validate blocks benchmarks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Fix number of issues with block benchmarks:
- correct block signing
- generating accounts correctly
- correctly get accounts by domain id
- remove account permissions on account removal
- update storage crate to fix issues with range iterator and removal of accounts 

## Benchmark results

After making account shallow we have the following result:

```plain
apply_blocks/apply_blocks
    time:   [18.491 ms 19.988 ms 21.691 ms]
    change: [+7.2201% +19.955% +34.299%] (p = 0.01 < 0.10)
    Performance has regressed.

validate_blocks/validate_blocks
    time:   [11.090 s 11.425 s 11.751 s]
    change: [-32.585% -29.986% -27.411%] (p = 0.00 < 0.10)
    Performance has improved.
```


<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

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
        Created At 2024-06-26 12:04:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4772" class=".btn">#4772</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump mypy from 1.10.0 to 1.10.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mypy](https://github.com/python/mypy) from 1.10.0 to 1.10.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python/mypy/blob/master/CHANGELOG.md">mypy's changelog</a>.</em></p>
<blockquote>
<h4>Mypy 1.10.1</h4>
<ul>
<li>Fix error reporting on cached run after uninstallation of third party library (Shantanu, PR <a href="https://redirect.github.com/python/mypy/pull/17420">17420</a>)</li>
</ul>
<h4>Acknowledgements</h4>
<p>Thanks to all mypy contributors who contributed to this release:</p>
<ul>
<li>Alex Waygood</li>
<li>Ali Hamdan</li>
<li>Edward Paget</li>
<li>Evgeniy Slobodkin</li>
<li>Hashem</li>
<li>hesam</li>
<li>Hugo van Kemenade</li>
<li>Ihor</li>
<li>James Braza</li>
<li>Jelle Zijlstra</li>
<li>jhance</li>
<li>Jukka Lehtosalo</li>
<li>Loïc Simon</li>
<li>Marc Mueller</li>
<li>Matthieu Devlin</li>
<li>Michael R. Crusoe</li>
<li>Nikita Sobolev</li>
<li>Oskari Lehto</li>
<li>Riccardo Di Maio</li>
<li>Richard Si</li>
<li>roberfi</li>
<li>Roman Solomatin</li>
<li>Sam Xifaras</li>
<li>Shantanu</li>
<li>Spencer Brown</li>
<li>Srinivas Lade</li>
<li>Tamir Duberstein</li>
<li>youkaichao</li>
</ul>
<p>I’d also like to thank my employer, Dropbox, for supporting mypy development.</p>
<h2>Mypy 1.9</h2>
<p>We’ve just uploaded mypy 1.9 to the Python Package Index (<a href="https://pypi.org/project/mypy/">PyPI</a>). Mypy is a static type checker for Python. This release includes new features, performance improvements and bug fixes. You can install it as follows:</p>
<pre><code>python3 -m pip install -U mypy
</code></pre>
<p>You can read the full documentation for this release on <a href="http://mypy.readthedocs.io">Read the Docs</a>.</p>
<h4>Breaking Changes</h4>
<p>Because the version of typeshed we use in mypy 1.9 doesn't support 3.7, neither does mypy 1.9. (Jared Hance, PR <a href="https://redirect.github.com/python/mypy/pull/16883">16883</a>)</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python/mypy/commit/c28b5257b528f65a028e7d0dbecbcd81c7997356"><code>c28b525</code></a> [1.10 backport] Fix error reporting on cached run after uninstallation of thi...</li>
<li>See full diff in <a href="https://github.com/python/mypy/compare/v1.10.0...v1.10.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mypy&package-manager=pip&previous-version=1.10.0&new-version=1.10.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-25 16:55:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4771" class=".btn">#4771</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_json from 1.0.117 to 1.0.118
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.117 to 1.0.118.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.118</h2>
<ul>
<li>Implement Hash for serde_json::Value (<a href="https://redirect.github.com/serde-rs/json/issues/1127">#1127</a>, thanks <a href="https://github.com/edwardycl"><code>@​edwardycl</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/c4f24f3be29a3d096d3ac7b1d5594777a613ec0d"><code>c4f24f3</code></a> Release 1.0.118</li>
<li><a href="https://github.com/serde-rs/json/commit/51d94ebdc07127de22fb655bdcf6a01d119492d5"><code>51d94eb</code></a> Combine Map's Hash into one impl</li>
<li><a href="https://github.com/serde-rs/json/commit/5e7bedc0a0e19ecda1c15a412ab7c69569f4aa84"><code>5e7bedc</code></a> Touch up PR 1127</li>
<li><a href="https://github.com/serde-rs/json/commit/0af2bdae9483a9c54f8e032fcbf357dbe7803c49"><code>0af2bda</code></a> Resolve semicolon_if_nothing_returned pedantic clippy lint from PR 1127</li>
<li><a href="https://github.com/serde-rs/json/commit/eb0330a178e0c179321101fbcbb5cb7530a2a3e5"><code>eb0330a</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1127">#1127</a> from edwardycl/hash</li>
<li><a href="https://github.com/serde-rs/json/commit/24d868f4e9be428afa1c744f8218a32660a1e0bf"><code>24d868f</code></a> Another lexical const that is unused, though not in test</li>
<li><a href="https://github.com/serde-rs/json/commit/4c894eaa18181860f3f5cf3fb11e18d4ee454120"><code>4c894ea</code></a> Delete unused associated constant from lexical</li>
<li><a href="https://github.com/serde-rs/json/commit/fa8aa223c66018cae73efa57fd276af329a343f4"><code>fa8aa22</code></a> Fill in ignore reasons in all #[ignore] attributes</li>
<li><a href="https://github.com/serde-rs/json/commit/c9b9f88c1add99e20fefcd377a29b00715b4e8c3"><code>c9b9f88</code></a> Run more of test suite in preserve_order mode</li>
<li><a href="https://github.com/serde-rs/json/commit/b83d243e711b65e32925510343df566080776dd5"><code>b83d243</code></a> Ignore large_digit_groups pedantic clippy lint in test</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/json/compare/v1.0.117...v1.0.118">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.117&new-version=1.0.118)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-25 16:32:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4768" class=".btn">#4768</a>
            </td>
            <td>
                <b>
                    docs(md): fix typos in CONTRIBUTING, iroha_2_whitepaper, hot-reload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs(md): fix typos in CONTRIBUTING, iroha_2_whitepaper, hot-reload
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-25 09:47:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4766" class=".btn">#4766</a>
            </td>
            <td>
                <b>
                    chore(deps): bump uuid from 1.8.0 to 1.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [uuid](https://github.com/uuid-rs/uuid) from 1.8.0 to 1.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/uuid-rs/uuid/releases">uuid's releases</a>.</em></p>
<blockquote>
<h2>1.9.0</h2>
<h2><code>Uuid::now_v7()</code> is guaranteed to be monotonic</h2>
<p>Before this release, <code>Uuid::now_v7()</code> would only use the millisecond-precision timestamp for ordering. It now also uses a global 42-bit counter that's re-initialized each millisecond so that the following will always pass:</p>
<pre lang="rust"><code>let a = Uuid::now_v7();
let b = Uuid::now_v7();
<p>assert!(a &lt; b);
</code></pre></p>
<h2>What's Changed</h2>
<ul>
<li>Add a get_node_id method for v1 and v6 UUIDs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/748">uuid-rs/uuid#748</a></li>
<li>Update atomic and zerocopy to latest by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/750">uuid-rs/uuid#750</a></li>
<li>Add repository field to uuid-macro-internal crate by <a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/752">uuid-rs/uuid#752</a></li>
<li>update docs to updated RFC (from 4122 to 9562) by <a href="https://github.com/Mikopet"><code>@​Mikopet</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/753">uuid-rs/uuid#753</a></li>
<li>Support counters in v7 UUIDs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/755">uuid-rs/uuid#755</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/paolobarbolini"><code>@​paolobarbolini</code></a> made their first contribution in <a href="https://redirect.github.com/uuid-rs/uuid/pull/752">uuid-rs/uuid#752</a></li>
<li><a href="https://github.com/Mikopet"><code>@​Mikopet</code></a> made their first contribution in <a href="https://redirect.github.com/uuid-rs/uuid/pull/753">uuid-rs/uuid#753</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/uuid-rs/uuid/compare/1.8.0...1.9.0">https://github.com/uuid-rs/uuid/compare/1.8.0...1.9.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/uuid-rs/uuid/commit/4a129e728174a340ac2772f3cc6310ba77d1969f"><code>4a129e7</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/760">#760</a> from uuid-rs/cargo/1.9.0</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/6bfee6ba82ad8e7a0155f3161157dc3ea3a5d552"><code>6bfee6b</code></a> prepare for 1.9.0 release</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/62b7145d95913642298d5a954314ea28a199fa78"><code>62b7145</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/759">#759</a> from uuid-rs/chore/v7-counter-cleanup</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/62e968c92b464c81a73b6002ab66a32c4bdad9ad"><code>62e968c</code></a> clean up new Timestamp APIs</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/49319a7ff766dc7c7638c0226294beebd45f6762"><code>49319a7</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/758">#758</a> from uuid-rs/chore/test-overflow</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/47b9130ada093391db900b03e53f716310ae1ca0"><code>47b9130</code></a> ensure v7 methods don't overflow on max values</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/0c561e3443191065b724e8f8eb7b116f08d4e181"><code>0c561e3</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/757">#757</a> from uuid-rs/ci/more-miri</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/252770be2f824e2cb4a2f68cb5980e0b7bd4b6cc"><code>252770b</code></a> expand miri tests to cover all features</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/e62647f7623f8663f806ec69d8264fbfb836a6e3"><code>e62647f</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/755">#755</a> from uuid-rs/feat/v7-counter</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/c270b3d66ae809517663ffeb38d56e004c517f7f"><code>c270b3d</code></a> improve testing for contexts</li>
<li>Additional commits viewable in <a href="https://github.com/uuid-rs/uuid/compare/1.8.0...1.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uuid&package-manager=cargo&previous-version=1.8.0&new-version=1.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-24 16:40:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4765" class=".btn">#4765</a>
            </td>
            <td>
                <b>
                    fix: restore RawGenesisTransaction schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
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
        Created At 2024-06-24 08:30:19 +0000 UTC
    </div>
</div>

