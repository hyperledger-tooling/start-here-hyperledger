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
                PR <a href="https://github.com/hyperledger/iroha/pull/4819" class=".btn">#4819</a>
            </td>
            <td>
                <b>
                    chore(deps): bump trybuild from 1.0.96 to 1.0.97
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [trybuild](https://github.com/dtolnay/trybuild) from 1.0.96 to 1.0.97.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/trybuild/releases">trybuild's releases</a>.</em></p>
<blockquote>
<h2>1.0.97</h2>
<ul>
<li>Normalize number of types listed in <em>&quot;the following other types implement trait&quot;</em> diagnostics (<a href="https://redirect.github.com/dtolnay/trybuild/issues/277">#277</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/trybuild/commit/daeef9c9b0b0da1c63eb9e2ce2b2cc816e0ddc8c"><code>daeef9c</code></a> Release 1.0.97</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/207b0a51a72de39d66aa09d4884ac8fbe2e529b7"><code>207b0a5</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/278">#278</a> from dtolnay/rustflags</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/1b8d4bdf0718bfe4719039ad2d3d53c9f5ccdab5"><code>1b8d4bd</code></a> Combine all rustflags into cargo --config arg</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/ef6893bf616cc6fd97264118473e45fbfeb27217"><code>ef6893b</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/trybuild/issues/277">#277</a> from dtolnay/nothers</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/883a38daa03e97053180f70e0b7b6446f1b7724a"><code>883a38d</code></a> Ignore comparison_chain clippy lint</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/f3b1dab3275e628d4e0b486d494fd820eb7bb559"><code>f3b1dab</code></a> Normalize the effect of --verbose on '$N others' diagnostic</li>
<li><a href="https://github.com/dtolnay/trybuild/commit/6184f60b31cf9547f2a2697c57a5852fc186d996"><code>6184f60</code></a> Add test of 'following other types' diagnostic</li>
<li>See full diff in <a href="https://github.com/dtolnay/trybuild/compare/1.0.96...1.0.97">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=trybuild&package-manager=cargo&previous-version=1.0.96&new-version=1.0.97)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:04:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4818" class=".btn">#4818</a>
            </td>
            <td>
                <b>
                    chore(deps): bump async-trait from 0.1.80 to 0.1.81
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [async-trait](https://github.com/dtolnay/async-trait) from 0.1.80 to 0.1.81.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/async-trait/releases">async-trait's releases</a>.</em></p>
<blockquote>
<h2>0.1.81</h2>
<ul>
<li>Turn off unneeded features of <code>syn</code> dependency (<a href="https://redirect.github.com/dtolnay/async-trait/issues/272">#272</a>, thanks <a href="https://github.com/klensy"><code>@​klensy</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/async-trait/commit/383f65f138963391a41d25ed7e2857fa002c5742"><code>383f65f</code></a> Release 0.1.81</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/4ec740e1dddab158a46f59271245984d1b92794d"><code>4ec740e</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/273">#273</a> from dtolnay/cloneimpls</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/b6c606384471c26a06852c0586304965237c0b95"><code>b6c6063</code></a> Ignore trivially_copy_pass_by_ref pedantic clippy lint</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/315fd9005c8294ecf2d9cce84d1d5a53da656b19"><code>315fd90</code></a> Turn off syn/clone-impls feature</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/94a3165a30a225c2d78425e4c68fc5ec67929a98"><code>94a3165</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/272">#272</a> from klensy/syn-f</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/2fac9405c8d3ecf8c08b0085ec338b72a643e43c"><code>2fac940</code></a> syn: remove derive feature</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/4a00d732460d37e219755bfc6db132b42b8c4af1"><code>4a00d73</code></a> Work around dead code warning in test</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/dba15b5a73f34a2fd96361a2fa8993ba412a43e1"><code>dba15b5</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/270">#270</a> from dtolnay/objsafety</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/d28c95b2037901ff4c36b631054d463f675f991c"><code>d28c95b</code></a> Former where_clauses_object_safety lint is now hard error</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/78a5922b4a9e81c72676dbeb9ea3bac50535864b"><code>78a5922</code></a> Fill in ignore reasons in all #[ignore] attributes</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/async-trait/compare/0.1.80...0.1.81">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async-trait&package-manager=cargo&previous-version=0.1.80&new-version=0.1.81)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:03:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4817" class=".btn">#4817</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.68 to 2.0.69
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.68 to 2.0.69.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.69</h2>
<ul>
<li>Correctly parenthesize labeled loops inside a break value (<a href="https://redirect.github.com/dtolnay/syn/issues/1692">#1692</a>)</li>
<li>Add <code>Punctuated::get</code> and <code>get_mut</code> (<a href="https://redirect.github.com/dtolnay/syn/issues/1693">#1693</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/d4a0ff556fe1bbcaa77ebc37d24cc1bdaf5eac3a"><code>d4a0ff5</code></a> Release 2.0.69</li>
<li><a href="https://github.com/dtolnay/syn/commit/0f7213407fb59cca90a1097747868b68b32ff020"><code>0f72134</code></a> Improve precedence variant name of sum and product operators</li>
<li><a href="https://github.com/dtolnay/syn/commit/06f34fce1a62e75fbd0400b93181ff989e16505b"><code>06f34fc</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1693">#1693</a> from dtolnay/get</li>
<li><a href="https://github.com/dtolnay/syn/commit/a4438571c902aae659ff568419fa4af029b5c0b0"><code>a443857</code></a> Add Punctuated::get and get_mut</li>
<li><a href="https://github.com/dtolnay/syn/commit/f0dfdbd9af41fe75ee6054daca545d80a4374a32"><code>f0dfdbd</code></a> Update test suite to nightly-2024-07-05</li>
<li><a href="https://github.com/dtolnay/syn/commit/1560f9a2ac7937fee688eaa98ad009caaeef323c"><code>1560f9a</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1692">#1692</a> from dtolnay/break</li>
<li><a href="https://github.com/dtolnay/syn/commit/4e71c1caa413122a644f9e3fcb8222dfc20d9f8d"><code>4e71c1c</code></a> Parenthesize labeled loops inside break value</li>
<li><a href="https://github.com/dtolnay/syn/commit/93931a4f243665a1e50748072b9fac1adbcebb7c"><code>93931a4</code></a> Add fixup test for break with leading label</li>
<li><a href="https://github.com/dtolnay/syn/commit/cc5e64e4143099699c5c7f20791c563e71395455"><code>cc5e64e</code></a> Update test suite to nightly-2024-06-29</li>
<li><a href="https://github.com/dtolnay/syn/commit/2bbf612a945f94860be6197c1efc76f8e3ae9e6c"><code>2bbf612</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1691">#1691</a> from dtolnay/postfix</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/syn/compare/2.0.68...2.0.69">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.68&new-version=2.0.69)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4816" class=".btn">#4816</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.203 to 1.0.204
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.203 to 1.0.204.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.204</h2>
<ul>
<li>Apply #[diagnostic::on_unimplemented] attribute on Rust 1.78+ to suggest adding serde derive or enabling a &quot;serde&quot; feature flag in dependencies (<a href="https://redirect.github.com/serde-rs/serde/issues/2767">#2767</a>, thanks <a href="https://github.com/weiznich"><code>@​weiznich</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/18dcae0a77632fb4767a420c550cb41991f750b8"><code>18dcae0</code></a> Release 1.0.204</li>
<li><a href="https://github.com/serde-rs/serde/commit/58c307f9cc28a19d73a0e2869f6addf9a8a329f9"><code>58c307f</code></a> Alphabetize list of rustc-check-cfg</li>
<li><a href="https://github.com/serde-rs/serde/commit/8cc4809414a83de0d41eac38ecfa1040e088b61e"><code>8cc4809</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2769">#2769</a> from dtolnay/onunimpl</li>
<li><a href="https://github.com/serde-rs/serde/commit/1179158defc5351467cbd2c340b7e1498391bce4"><code>1179158</code></a> Update ui test with diagnostic::on_unimplemented from PR 2767</li>
<li><a href="https://github.com/serde-rs/serde/commit/91aa40e749620f31bf7db01c772e672f023136b5"><code>91aa40e</code></a> Add ui test of unsatisfied serde trait bound</li>
<li><a href="https://github.com/serde-rs/serde/commit/595019e979ebed5452b550bf901abcab2cf4e945"><code>595019e</code></a> Cut test_suite from workspace members in old toolchain CI jobs</li>
<li><a href="https://github.com/serde-rs/serde/commit/b0d7917f88978eda264f8fbac13b46ece35f5348"><code>b0d7917</code></a> Pull in trybuild 'following types implement trait' fix</li>
<li><a href="https://github.com/serde-rs/serde/commit/8e6637a1e44c30dffd37322a7107d434cd751722"><code>8e6637a</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2767">#2767</a> from weiznich/feature/diagnostic_on_unimplemented</li>
<li><a href="https://github.com/serde-rs/serde/commit/694fe0595358aa0857120a99041d99975b1a8a70"><code>694fe05</code></a> Use the <code>#[diagnostic::on_unimplemented]</code> attribute when possible</li>
<li><a href="https://github.com/serde-rs/serde/commit/f3dfd2a2375d9caf15a18ec657dde51a32caf6ed"><code>f3dfd2a</code></a> Suppress dead code warning in test of unit struct remote derive</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/serde/compare/v1.0.203...v1.0.204">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.203&new-version=1.0.204)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 17:02:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4812" class=".btn">#4812</a>
            </td>
            <td>
                <b>
                    feat!: speicfy on-chain parameters explicitly in genesis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Currently it's not possible to submit genesis which doesn't pass under default parameter values (i.e. large genesis). 
This PR fixes that allowing to specify parameters inside genesis.json so that they are applied before processing rest of instructions.

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
        Created At 2024-07-08 11:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4810" class=".btn">#4810</a>
            </td>
            <td>
                <b>
                    refactor!: rename wasm to smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

The fact that we work with wasm smart contracts is a sort of implementation detail.
Let's not specify implementation details in the API.


### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

If we change from wasm to some other VM, we will have a reduced effect on the API.
If we don't it is implied that we use wasm, so no harm done there

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
        Created At 2024-07-08 08:50:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4809" class=".btn">#4809</a>
            </td>
            <td>
                <b>
                    refactor!: remove `FindAssetsByName` query
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

Closes #3720

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
        Created At 2024-07-08 08:49:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4808" class=".btn">#4808</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_with from 3.8.2 to 3.8.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_with](https://github.com/jonasbb/serde_with) from 3.8.2 to 3.8.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonasbb/serde_with/releases">serde_with's releases</a>.</em></p>
<blockquote>
<h2>serde_with v3.8.3</h2>
<h3>Fixed</h3>
<ul>
<li>Fix compile issues when dependency <code>schemars_0_8</code> is used with the <code>preserve_order</code> features (<a href="https://redirect.github.com/jonasbb/serde_with/issues/762">#762</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonasbb/serde_with/commit/1c4b022e6018fbf1f9cb2e897bae519f91ed6908"><code>1c4b022</code></a> Bump version to v3.8.3 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/765">#765</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/7de983895c0dcbf8598676f52b987a0026f7d816"><code>7de9838</code></a> Bump version to v3.8.3</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/19bfe182439616416f0fc17b1fac134e1b29e537"><code>19bfe18</code></a> Make code compile with <code>schemars_0_8/preserve_order</code> enabled (<a href="https://redirect.github.com/jonasbb/serde_with/issues/764">#764</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/4c8c2db1105da0408c89330e0bcfc7ac4818975c"><code>4c8c2db</code></a> Make code compile with <code>schemars_0_8/preserve_order</code> enabled</li>
<li>See full diff in <a href="https://github.com/jonasbb/serde_with/compare/v3.8.2...v3.8.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_with&package-manager=cargo&previous-version=3.8.2&new-version=3.8.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-05 16:29:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4807" class=".btn">#4807</a>
            </td>
            <td>
                <b>
                    fix: Check that authority owns domain to transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

When transfer `domain` from `source` account:
* Fixed check in executor that `authority` owns `domain` (previously it checked that `source` owns `domain`, but it is not needed since it is checked in iroha_core)
* Improved error message for check that `source` owns `domain` in iroha_core

### Linked issue

Closes #4751

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2024-07-05 14:53:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4806" class=".btn">#4806</a>
            </td>
            <td>
                <b>
                    feat: include parameters into generated genesis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Include parameters into default genesis.json.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

While parameters may have default values i still think it's useful to include them into default genesis as an example.
I've got contacted by our QA and they didn't have a way to know how new parameters are expressed in the genesis.

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
        Created At 2024-07-05 09:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4805" class=".btn">#4805</a>
            </td>
            <td>
                <b>
                    refactor(client): allow turbofish with multiple `Instruction`s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Converts `impl Instruction` to an explicit type parameter in functions accepting multiple instructions.

### Benefits

Lets users avoid converting heterogeneous instructions to `InstructionBox`es in a separate variable before submitting to a client, which is more ergonomic.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2024-07-05 09:13:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4804" class=".btn">#4804</a>
            </td>
            <td>
                <b>
                    fix: Fix failing tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Fix those tests:
* `iroha::mod integration::upgrade::migration_should_cause_upgrade_event`
* `iroha_core queue::tests::queue_throttling`
* `iroha_core smartcontracts::isi::query::tests::asset_store`
* `parity_scale_cli::bin/parity_scale_cli tests::decode_account_sample`
* `parity_scale_cli::bin/parity_scale_cli tests::decode_domain_sample`

### Linked issue

### Benefits

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
        Created At 2024-07-04 12:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4802" class=".btn">#4802</a>
            </td>
            <td>
                <b>
                    fix: Smarter transaction expire logic
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
        Created At 2024-07-04 07:05:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4801" class=".btn">#4801</a>
            </td>
            <td>
                <b>
                    chore: add `a-zorina` to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 06:47:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4800" class=".btn">#4800</a>
            </td>
            <td>
                <b>
                    fix(validate_blocks): remove loger double initialiation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Fix error with double initialization of logger.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 11:05:40 +0000 UTC
    </div>
</div>

