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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4799" class=".btn">#4799</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_json from 1.0.118 to 1.0.120
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.118 to 1.0.120.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.120</h2>
<ul>
<li>Correctly specify required version of <code>indexmap</code> dependency (<a href="https://redirect.github.com/serde-rs/json/issues/1152">#1152</a>, thanks <a href="https://github.com/cforycki"><code>@​cforycki</code></a>)</li>
</ul>
<h2>v1.0.119</h2>
<ul>
<li>Add <code>serde_json::Map::shift_insert</code> (<a href="https://redirect.github.com/serde-rs/json/issues/1149">#1149</a>, thanks <a href="https://github.com/joshka"><code>@​joshka</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/bcedc3d96bcc33184f16d63eab397295e2193350"><code>bcedc3d</code></a> Release 1.0.120</li>
<li><a href="https://github.com/serde-rs/json/commit/962c0fbbecc7dc8559cfeb019c2611737512f937"><code>962c0fb</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1152">#1152</a> from cforycki/fix/index-map-minimal-version</li>
<li><a href="https://github.com/serde-rs/json/commit/3480feda7b572d33992544061a8e0fbf8610a803"><code>3480fed</code></a> fix: indexmap minimal version with Map::shift_insert()</li>
<li><a href="https://github.com/serde-rs/json/commit/b48b9a3a0c09952579e98c8940fe0d1ee4aae588"><code>b48b9a3</code></a> Release 1.0.119</li>
<li><a href="https://github.com/serde-rs/json/commit/8878cd7c042a5f94ae4ee9889cbcbd12cc5ce334"><code>8878cd7</code></a> Make shift_insert available for inlining like other Map methods</li>
<li><a href="https://github.com/serde-rs/json/commit/352b7abf007cf3b9b063b01e0b1e8f6af62a4e39"><code>352b7ab</code></a> Document the cfg required for Map::shift_insert to exist</li>
<li><a href="https://github.com/serde-rs/json/commit/c17e63f6eff6cb40594beb1bddd4562c4cc81442"><code>c17e63f</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1149">#1149</a> from joshka/master</li>
<li><a href="https://github.com/serde-rs/json/commit/309ef6b8870e47622a283061cbda3f5514bfaf0d"><code>309ef6b</code></a> Add Map::shift_insert()</li>
<li><a href="https://github.com/serde-rs/json/commit/a9e089a2ce245bc223b56fbb6c525e2fe7b1f0ef"><code>a9e089a</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1146">#1146</a> from haouvw/master</li>
<li><a href="https://github.com/serde-rs/json/commit/a83fe96ae2a202925f1caa7abc51991f321d7c22"><code>a83fe96</code></a> chore: remove repeat words</li>
<li>See full diff in <a href="https://github.com/serde-rs/json/compare/v1.0.118...v1.0.120">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.118&new-version=1.0.120)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 18:13:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4797" class=".btn">#4797</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_with from 3.8.1 to 3.8.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_with](https://github.com/jonasbb/serde_with) from 3.8.1 to 3.8.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonasbb/serde_with/releases">serde_with's releases</a>.</em></p>
<blockquote>
<h2>serde_with v3.8.2</h2>
<h3>Changed</h3>
<ul>
<li>Bump MSRV to 1.67, since that is required for the <code>time</code> dependency.
The <code>time</code> version needed to be updated for nightly compatibility.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Implement <code>JsonSchemaAs</code> for <code>OneOrMany</code> instead of <code>JsonSchema</code> by <a href="https://github.com/swlynch99"><code>@​swlynch99</code></a> (<a href="https://redirect.github.com/jonasbb/serde_with/issues/760">#760</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonasbb/serde_with/commit/2274dd142afbd6788ad43cba7f66710af78c4e03"><code>2274dd1</code></a> Bump version to 3.8.2 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/761">#761</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/e9e7a7e99c8d49cdc335203418ca858b9d0d2a92"><code>e9e7a7e</code></a> Bump version to 3.8.2</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/c9d96723876291a6d2830d7d50f0382a11805c28"><code>c9d9672</code></a> Implement JsonSchemaAs for OneOrMany instead of JsonSchema (<a href="https://redirect.github.com/jonasbb/serde_with/issues/760">#760</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/dee706a528cb37f853be5bd2b6b4c2b3605eab80"><code>dee706a</code></a> Implement JsonSchemaAs for OneOrMany instead of JsonSchema</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/f74b460e69535738b876bd8f52bacc499cfe7228"><code>f74b460</code></a> Fix two clippy issues (<a href="https://redirect.github.com/jonasbb/serde_with/issues/755">#755</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/3ae442485e34c8b0c3c34fa3c953fa77e0a1a19d"><code>3ae4424</code></a> Fix two clippy issues</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/729e8d23eaf013d9de8b3806b7f574901009af56"><code>729e8d2</code></a> Replace future deprecated functions from chrono (<a href="https://redirect.github.com/jonasbb/serde_with/issues/752">#752</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/685338f44f01eaefdbdb40fc7a636d113e693916"><code>685338f</code></a> Replace future deprecated functions from chrono</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/9593f932721046e2a50a0c761ee43634d7c9517b"><code>9593f93</code></a> Enable the <code>unexpected_cfgs</code> lint now that it can be configured via `Cargo.to...</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/242286c52bc2210da3863e3bc9e71c142f67b788"><code>242286c</code></a> Enable the <code>unexpected_cfgs</code> lint now that it can be configured via <code>Cargo.toml</code></li>
<li>Additional commits viewable in <a href="https://github.com/jonasbb/serde_with/compare/v3.8.1...v3.8.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_with&package-manager=cargo&previous-version=3.8.1&new-version=3.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 16:19:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4796" class=".btn">#4796</a>
            </td>
            <td>
                <b>
                    chore(deps): bump clap from 4.5.7 to 4.5.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [clap](https://github.com/clap-rs/clap) from 4.5.7 to 4.5.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/releases">clap's releases</a>.</em></p>
<blockquote>
<h2>v4.5.8</h2>
<h2>[4.5.8] - 2024-06-28</h2>
<h3>Fixes</h3>
<ul>
<li>Reduce extra flushes</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/clap-rs/clap/blob/master/CHANGELOG.md">clap's changelog</a>.</em></p>
<blockquote>
<h2>[4.5.8] - 2024-06-28</h2>
<h3>Fixes</h3>
<ul>
<li>Reduce extra flushes</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/clap-rs/clap/compare/clap_complete-v4.5.7...v4.5.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clap&package-manager=cargo&previous-version=4.5.7&new-version=4.5.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 16:18:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4794" class=".btn">#4794</a>
            </td>
            <td>
                <b>
                    refactor(swarm): build with `irohad0` instead of dummy builder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Image for Compose is now built by the first peer service instead of the dummy builder. Solves [the CI failure](https://github.com/hyperledger/iroha/actions/runs/9739223415/job/26874072004) when testing generated Compose configs caused by https://github.com/docker/compose/issues/10596.

### Benefits

No need for a dummy service to build images.

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
        Created At 2024-07-01 10:36:55 +0000 UTC
    </div>
</div>

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
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

* remove `derive` crates from workspace dependencies
* split `executor` into `data_model` and `core` crates 
* rewrite tests/examples so that they use statically typed permissions
* removed `MigrationResult` -> migration should always succeed, the error is unrecoverable

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue
 #4552

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

