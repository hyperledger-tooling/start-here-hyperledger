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

