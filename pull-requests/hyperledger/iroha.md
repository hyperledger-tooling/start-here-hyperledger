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
                PR <a href="https://github.com/hyperledger/iroha/pull/4673" class=".btn">#4673</a>
            </td>
            <td>
                <b>
                    refactor!: Remove genesis signing from Iroha
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Implementation of https://github.com/hyperledger/iroha/issues/4225#issuecomment-2087976958 partially based on #4382.

This PR includes:
* New `kagami genesis sign` command to sign and transform `genesis.json` into `signed-genesis.scale` (SCALE serialized `SignedTransaction`)
* Changes in config:
  * `genesis.private_key` removed
  * `genesis.file` renamed to `genesis.signed_file`
* Changes in swarm: added signing genesis with kagami before starting peer

Things left for future PRs:
* Remove `--submit-genesis` CLI argument and make all peers submit genesis ?
* Small refactoring - remove/inline `GenesisNetwork` struct (it always contains only one `GenesisTransaction`)

### Linked issue

Closes #4225
Closes #4382

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
        Created At 2024-05-30 15:56:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4671" class=".btn">#4671</a>
            </td>
            <td>
                <b>
                    fix: Fix test `no_extra_or_missing_schemas`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated schema types to fix test `no_extra_or_missing_schemas`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 14:03:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4668" class=".btn">#4668</a>
            </td>
            <td>
                <b>
                    feat!: recognize and activate accounts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">api-changes</span>
            </td>
            <td>
                BREAKING_CHANGE:

- `Account` contains `is_active` field
- `AccountEvent::Created` divides into `Recognized` and `Activated`
- `ValidationFail` contains `UnrecognizedAuthority` and `InactiveAuthority` variants

## Description

When an account is _recognized_,

- it becomes able to hold assets, permissions, roles, and metadata
- it cannot yet execute any queries or transactions

When an account is _activated_,

- it becomes able to execute queries and transactions

Recognize and activate an account when targeted as:

- `Register<Account>` object

Recognize an account when targeted as:

- `Register<Asset>` object.account
- `Mint<Numeric, Asset>` destination.account
- ~~`Transfer<Account, DomainId, Account>` destination~~ See [comment](https://github.com/hyperledger/iroha/pull/4668#discussion_r1619777320)
- `Transfer<Account, AssetDefinitionId, Account>` destination
- `Transfer<Asset, Numeric, Account>` destination
- `Transfer<Asset, Metadata, Account>` destination
- `SetKeyValue<Account>` object
- `SetKeyValue<Asset>` object.account
- `Grant<Permission, Account>` destination
- `Grant<Role, Account>` destination

Let me call these _creative instructions_ in documentation

### Linked issue

- closes #4426

### Benefits

- who targets an account does not need to care if it has been registered or not
- depending on use case, accounts can be registered implicitly/automatically or explicitly/manually

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
        Created At 2024-05-30 03:01:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4667" class=".btn">#4667</a>
            </td>
            <td>
                <b>
                    refactor!: revert `_ms` and `_bytes` suffixes in config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Since there is still no consensus about using human readable types in configuration (#4294, #4295), I decided to at least make it explicit that they aren't supported.

- Reverted use of `_ms` suffix for millisecond numbers
- Used `_bytes` suffix for <code>torii.max_content_length<b>_bytes</b></code>
- Updated config templates
- Refactored internals:
  - Renamed `HumanDuration` to `DurationMs`, and `HumanBytes` to just `Bytes`
  - Chore refactors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 02:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4666" class=".btn">#4666</a>
            </td>
            <td>
                <b>
                    fix: avoid early drop of `ConfigReader` in `iroha_client` (#4623)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span>
            </td>
            <td>
                ## Description

Fixed usage of `ConfigReader` in `iroha_client`.

### Linked issue

Closes #4623

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 01:57:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4665" class=".btn">#4665</a>
            </td>
            <td>
                <b>
                    fix: Fix test `generate_peers_deterministically`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix test `generate_peers_deterministically` after `iroha` → `irohad` renaming (#4662)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-29 16:11:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4663" class=".btn">#4663</a>
            </td>
            <td>
                <b>
                    chore(deps): bump faker from 25.2.0 to 25.3.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 25.2.0 to 25.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v25.3.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v25.3.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v25.2.0...v25.3.0">v25.3.0 - 2024-05-28</a></h3>
<ul>
<li>Add more iOS versions to <code>user_agent</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/e0e0460ff715032ad5eda184d2fcb3720ce26b9c"><code>e0e0460</code></a> Bump version: 25.2.0 → 25.3.0</li>
<li><a href="https://github.com/joke2k/faker/commit/3497f21cceea485410927696358bb0de0218ce64"><code>3497f21</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/4cba6ee90e2637e66d3a7fb64b4aa71f6f5f1b21"><code>4cba6ee</code></a> Add more iOS versions to <code>user_agent</code> (<a href="https://redirect.github.com/joke2k/faker/issues/2032">#2032</a>)</li>
<li>See full diff in <a href="https://github.com/joke2k/faker/compare/v25.2.0...v25.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=25.2.0&new-version=25.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-28 16:10:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4662" class=".btn">#4662</a>
            </td>
            <td>
                <b>
                    refactor!: rename iroha server and client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

* rename `iroha` crate and binary to `irohad`
* rename `iroha_client_cli` binary to `iroha`
* rename `iroha_client` crate and binary to `iroha`

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4512

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
        Created At 2024-05-28 15:33:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4661" class=".btn">#4661</a>
            </td>
            <td>
                <b>
                    fix(BACKPORT): compare permission payloads as `serde_json::Value`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
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
        Created At 2024-05-28 12:20:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4660" class=".btn">#4660</a>
            </td>
            <td>
                <b>
                    chore(debug): Improve deserialization error message
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
        Created At 2024-05-28 11:31:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4659" class=".btn">#4659</a>
            </td>
            <td>
                <b>
                    chore(debug): improve deserialization error message
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
        Created At 2024-05-28 11:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4658" class=".btn">#4658</a>
            </td>
            <td>
                <b>
                    feat!: generalize permissions schema to executor data model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

This is a version of #4597, but without changing anything about parameters. What to do with parameters is not yet clear.

### Benefits

Gives a foundation for executor-defined...

- Parameters: #4352 
- Instructions: #4599 and #4645 
- Metadata: #4353 

### Linked issue

None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-28 01:36:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4657" class=".btn">#4657</a>
            </td>
            <td>
                <b>
                    ci: Remove coveralls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

1. Remove coveralls tool for coverage since it's useless while having it in the workflow trigger type (btw, it's still might be possible to fix). However, coverage is uploading in Sonarqube now.
2. Modify concurrency.
3. Run clippy and lcov jobs in the head branch context.
4. Remove defecdojo output print.
5. Trigger workflow within one parent workflow onlyto reduce parallel jobs creation.


### Benefits

Remove coveralls that doesn't work.
Reduce the possible amount of parallel runs of I2::Dev::CodeQuality workflow.

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
        Created At 2024-05-27 20:06:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4656" class=".btn">#4656</a>
            </td>
            <td>
                <b>
                    chore(deps): bump alpine from 3.19 to 3.20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps alpine from 3.19 to 3.20.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=alpine&package-manager=docker&previous-version=3.19&new-version=3.20)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4655" class=".btn">#4655</a>
            </td>
            <td>
                <b>
                    chore(deps): bump libsodium-sys-stable from 1.20.7 to 1.20.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [libsodium-sys-stable](https://github.com/jedisct1/libsodium-sys-stable) from 1.20.7 to 1.20.9.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/398d1f1a23027db3abe87813a6f5d73680323983"><code>398d1f1</code></a> Update to libsodium 1.0.20</li>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/2da70a0da6789374ca36d9a152b29d3ce0f992da"><code>2da70a0</code></a> Update libsodium</li>
<li>See full diff in <a href="https://github.com/jedisct1/libsodium-sys-stable/compare/1.20.7...1.20.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=libsodium-sys-stable&package-manager=cargo&previous-version=1.20.7&new-version=1.20.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:37:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4654" class=".btn">#4654</a>
            </td>
            <td>
                <b>
                    chore(deps): bump proc-macro2 from 1.0.83 to 1.0.84
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [proc-macro2](https://github.com/dtolnay/proc-macro2) from 1.0.83 to 1.0.84.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/proc-macro2/releases">proc-macro2's releases</a>.</em></p>
<blockquote>
<h2>1.0.84</h2>
<ul>
<li>Documentation improvements (<a href="https://redirect.github.com/dtolnay/proc-macro2/issues/455">#455</a>, thanks <a href="https://github.com/CensoredUsername"><code>@​CensoredUsername</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/33c95785826bbd1fa353c48989dfc5a7ca62f54c"><code>33c9578</code></a> Release 1.0.84</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/d850da5cf78a7705185e2c37c1269fb3e8c8d042"><code>d850da5</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/proc-macro2/issues/455">#455</a> from CensoredUsername/master</li>
<li><a href="https://github.com/dtolnay/proc-macro2/commit/eabac1560e2f672172623bf79e1cb8b5a9d1fe98"><code>eabac15</code></a> Add a warning to Delimiter::None that rustc currently does not respect it.</li>
<li>See full diff in <a href="https://github.com/dtolnay/proc-macro2/compare/1.0.83...1.0.84">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=proc-macro2&package-manager=cargo&previous-version=1.0.83&new-version=1.0.84)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4653" class=".btn">#4653</a>
            </td>
            <td>
                <b>
                    chore(deps): bump zeroize from 1.7.0 to 1.8.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [zeroize](https://github.com/RustCrypto/utils) from 1.7.0 to 1.8.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/RustCrypto/utils/commit/7050a8402b44344023cd8d27fe6e0e4055d6bdde"><code>7050a84</code></a> zeroize v1.8.1 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1075">#1075</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/4b7b782b89800109dfa51d1fbdd7389d607dcdaa"><code>4b7b782</code></a> zeroize: move <code>zeroize_derive</code> to toplevel (<a href="https://redirect.github.com/RustCrypto/utils/issues/1074">#1074</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/6b341bbacc58e6bfc1c260bbc88a7ca19221ef6f"><code>6b341bb</code></a> zeroize: feature-gate AVX-512 under <code>simd</code>; MSRV 1.60 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1073">#1073</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/f46a14777a6cb1c553dcc6dbdce26de8e1baf04e"><code>f46a147</code></a> zeroize: note v1.8.0 was yanked in CHANGELOG.md (<a href="https://redirect.github.com/RustCrypto/utils/issues/1071">#1071</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/a7eddc620ed683216b97d924deeab7ea4f84a5af"><code>a7eddc6</code></a> zeroize: fix unnecessary qualifications (<a href="https://redirect.github.com/RustCrypto/utils/issues/1072">#1072</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/9bbfb49e6541d710aea6f7a95c68c9f3d99140e2"><code>9bbfb49</code></a> zeroize 1.8.0 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1065">#1065</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/c0eab7f7abfc244e9fcd482520542329da31f87c"><code>c0eab7f</code></a> cpufeatures: fix macOS build (<a href="https://redirect.github.com/RustCrypto/utils/issues/1066">#1066</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/6d383a554b76df2c6796d8d2982a6a8535342617"><code>6d383a5</code></a> zeroize: always enable AArch64 support (<a href="https://redirect.github.com/RustCrypto/utils/issues/1064">#1064</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/24decb93793936110ae564b6c8e475d91f4e4e44"><code>24decb9</code></a> zeroize: use <code>doc_auto_cfg</code> (<a href="https://redirect.github.com/RustCrypto/utils/issues/1063">#1063</a>)</li>
<li><a href="https://github.com/RustCrypto/utils/commit/cd3a147d62f5f2bf8d5bd10185a52c90f842395b"><code>cd3a147</code></a> build(deps): bump prettyplease from 0.2.16 to 0.2.19 (<a href="https://redirect.github.com/RustCrypto/utils/issues/1061">#1061</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/RustCrypto/utils/compare/zeroize-v1.7.0...zeroize-v1.8.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=zeroize&package-manager=cargo&previous-version=1.7.0&new-version=1.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:36:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4652" class=".btn">#4652</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.202 to 1.0.203
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde](https://github.com/serde-rs/serde) from 1.0.202 to 1.0.203.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/serde/releases">serde's releases</a>.</em></p>
<blockquote>
<h2>v1.0.203</h2>
<ul>
<li>Documentation improvements (<a href="https://redirect.github.com/serde-rs/serde/issues/2747">#2747</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/serde/commit/d5bc546ca53be0b31984a06a8ad587cbea4ca5ce"><code>d5bc546</code></a> Release 1.0.203</li>
<li><a href="https://github.com/serde-rs/serde/commit/45ae217728e9163103c47f9bd04502368caaf446"><code>45ae217</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2747">#2747</a> from dtolnay/variadic</li>
<li><a href="https://github.com/serde-rs/serde/commit/b7b97dda7333baf6474517e3646754be54e3796b"><code>b7b97dd</code></a> Unindent implementation inside tuple_impl_body macro</li>
<li><a href="https://github.com/serde-rs/serde/commit/5d3c563d469ef36ce5a01f1612f53883fee20db5"><code>5d3c563</code></a> Document tuple impls as fake variadic</li>
<li><a href="https://github.com/serde-rs/serde/commit/376185458b48aeb2774ecc26422cc9499e564117"><code>3761854</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/serde/issues/2745">#2745</a> from dtolnay/docsrs</li>
<li><a href="https://github.com/serde-rs/serde/commit/a8f14840ab3ff58f533cd27d0f91955d57f12a65"><code>a8f1484</code></a> Rely on docs.rs to define --cfg=docsrs by default</li>
<li>See full diff in <a href="https://github.com/serde-rs/serde/compare/v1.0.202...v1.0.203">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde&package-manager=cargo&previous-version=1.0.202&new-version=1.0.203)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:35:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4651" class=".btn">#4651</a>
            </td>
            <td>
                <b>
                    chore(deps): bump parking_lot from 0.12.2 to 0.12.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [parking_lot](https://github.com/Amanieu/parking_lot) from 0.12.2 to 0.12.3.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/Amanieu/parking_lot/blob/master/CHANGELOG.md">parking_lot's changelog</a>.</em></p>
<blockquote>
<h2>parking_lot 0.12.3 (2024-05-24)</h2>
<ul>
<li>Export types provided by arc_lock feature (<a href="https://redirect.github.com/Amanieu/parking_lot/issues/442">#442</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Amanieu/parking_lot/commit/a29dd3d4ff661f73fd5cf638584bc4c5de2ad347"><code>a29dd3d</code></a> Release parking_lot 0.12.3</li>
<li><a href="https://github.com/Amanieu/parking_lot/commit/f7efcae51161c25f7839cddd20cc1b809441e5e8"><code>f7efcae</code></a> Merge pull request <a href="https://redirect.github.com/Amanieu/parking_lot/issues/442">#442</a> from iwanders/add-arc_lock-feature-top-level-exports</li>
<li><a href="https://github.com/Amanieu/parking_lot/commit/c357017decfa0f21ca597a4958745ad0999cf9eb"><code>c357017</code></a> Export types provided by arc_lock feature.</li>
<li>See full diff in <a href="https://github.com/Amanieu/parking_lot/compare/0.12.2...0.12.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=parking_lot&package-manager=cargo&previous-version=0.12.2&new-version=0.12.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-27 16:34:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4650" class=".btn">#4650</a>
            </td>
            <td>
                <b>
                    fix(crypto): do not panic if the passed Ed25519Sha512 public key is of invalid length
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Change the conversion of unsized slice to array reference to be infallible and form a better error message.

This prevents a panic during `parity_scale_cli`'s type probing

### Linked issue

Closes #4649 

### Checklist

- [ ] make CI pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-27 14:14:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4647" class=".btn">#4647</a>
            </td>
            <td>
                <b>
                    refactor: replace u64 with usize internally
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

would you welcome this change?

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
        Created At 2024-05-27 11:26:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4646" class=".btn">#4646</a>
            </td>
            <td>
                <b>
                    chore: update CODEOWNERS
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
        Created At 2024-05-27 06:58:12 +0000 UTC
    </div>
</div>

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

