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
                PR <a href="https://github.com/hyperledger/iroha/pull/4678" class=".btn">#4678</a>
            </td>
            <td>
                <b>
                    fix: Fix invalid value for profile.profiling.debug in Cargo.toml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The  key in the Cargo.toml  file was assigned an invalid value, causing the manifest parsing to fail. This commit updates the value to a valid boolean () to resolve the issue.

Fixes #4677

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4677

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Installation succeeds with `cargo build`.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up

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
        Created At 2024-05-31 23:48:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4676" class=".btn">#4676</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tokio from 1.37.0 to 1.38.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.37.0 to 1.38.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.38.0</h2>
<p>This release marks the beginning of stabilization for runtime metrics. It
stabilizes <code>RuntimeMetrics::worker_count</code>. Future releases will continue to
stabilize more metrics.</p>
<h3>Added</h3>
<ul>
<li>fs: add <code>File::create_new</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6573">#6573</a>)</li>
<li>io: add <code>copy_bidirectional_with_sizes</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6500">#6500</a>)</li>
<li>io: implement <code>AsyncBufRead</code> for <code>Join</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6449">#6449</a>)</li>
<li>net: add Apple visionOS support (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6465">#6465</a>)</li>
<li>net: implement <code>Clone</code> for <code>NamedPipeInfo</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6586">#6586</a>)</li>
<li>net: support QNX OS (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6421">#6421</a>)</li>
<li>sync: add <code>Notify::notify_last</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6520">#6520</a>)</li>
<li>sync: add <code>mpsc::Receiver::{capacity,max_capacity}</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6511">#6511</a>)</li>
<li>sync: add <code>split</code> method to the semaphore permit (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6472">#6472</a>, <a href="https://redirect.github.com/tokio-rs/tokio/issues/6478">#6478</a>)</li>
<li>task: add <code>tokio::task::join_set::Builder::spawn_blocking</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6578">#6578</a>)</li>
<li>wasm: support rt-multi-thread with wasm32-wasi-preview1-threads (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6510">#6510</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>macros: make <code>#[tokio::test]</code> append <code>#[test]</code> at the end of the attribute list (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6497">#6497</a>)</li>
<li>metrics: fix <code>blocking_threads</code> count (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6551">#6551</a>)</li>
<li>metrics: stabilize <code>RuntimeMetrics::worker_count</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6556">#6556</a>)</li>
<li>runtime: move task out of the <code>lifo_slot</code> in <code>block_in_place</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6596">#6596</a>)</li>
<li>runtime: panic if <code>global_queue_interval</code> is zero (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6445">#6445</a>)</li>
<li>sync: always drop message in destructor for oneshot receiver (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6558">#6558</a>)</li>
<li>sync: instrument <code>Semaphore</code> for task dumps (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6499">#6499</a>)</li>
<li>sync: use FIFO ordering when waking batches of wakers (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6521">#6521</a>)</li>
<li>task: make <code>LocalKey::get</code> work with Clone types (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6433">#6433</a>)</li>
<li>tests: update nix and mio-aio dev-dependencies (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6552">#6552</a>)</li>
<li>time: clean up implementation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6517">#6517</a>)</li>
<li>time: lazily init timers on first poll (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6512">#6512</a>)</li>
<li>time: remove the <code>true_when</code> field in <code>TimerShared</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6563">#6563</a>)</li>
<li>time: use sharding for timer implementation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6534">#6534</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>taskdump: allow building taskdump docs on non-unix machines (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6564">#6564</a>)</li>
<li>time: check for overflow in <code>Interval::poll_tick</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6487">#6487</a>)</li>
<li>sync: fix incorrect <code>is_empty</code> on mpsc block boundaries (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6603">#6603</a>)</li>
</ul>
<h3>Documented</h3>
<ul>
<li>fs: rewrite file system docs (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6467">#6467</a>)</li>
<li>io: fix <code>stdin</code> documentation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6581">#6581</a>)</li>
<li>io: fix obsolete reference in <code>ReadHalf::unsplit()</code> documentation (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6498">#6498</a>)</li>
<li>macros: render more comprehensible documentation for <code>select!</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6468">#6468</a>)</li>
<li>net: add missing types to module docs (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6482">#6482</a>)</li>
<li>net: fix misleading <code>NamedPipeServer</code> example (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6590">#6590</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/14c17fc09656a30230177b600bacceb9db33e942"><code>14c17fc</code></a> chore: prepare Tokio v1.38.0 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6601">#6601</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/65cbf730de48ef9d3c84959d26ab717a85a5de62"><code>65cbf73</code></a> chore: prepare tokio-macros v2.3.0 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6600">#6600</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/dbf93c71844a01574a10f9dee0d4d9655a569f0a"><code>dbf93c7</code></a> sync: fix incorrect is_empty on mpsc block boundaries (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6603">#6603</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/873cb8ae2fc291eaffbd71e3c83d17b2f0ed7abf"><code>873cb8a</code></a> runtime: move task out of the <code>lifo_slot</code> in <code>block_in_place</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6596">#6596</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/97bb47b480c66083397c21d54e7ae33cab6c1b20"><code>97bb47b</code></a> task: fix a typo in doc of <code>LocalSet::run_until</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6599">#6599</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/86658bd87dc470f8e36eb6b893cc403820cfb7ee"><code>86658bd</code></a> metrics: stabilize <code>RuntimeMetrics::worker_count</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6556">#6556</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9e00b266e08d263c497dc9de57d9acbc049ae69b"><code>9e00b26</code></a> sync: add <code>Notify::notify_last</code> (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6520">#6520</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/6c42d286b343f498ce29de2aab9358a0aedb081c"><code>6c42d28</code></a> net: fix misleading <code>NamedPipeServer</code> example (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6590">#6590</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/3a6fdc05681841c30fe4e27b63924c7908ea4634"><code>3a6fdc0</code></a> license: fix formatting and remove year in licenses (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6451">#6451</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/2890d0c3db4f595330d8d223bfbfeb81e205b048"><code>2890d0c</code></a> metrics: fix blocking_threads count (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6551">#6551</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.37.0...tokio-1.38.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.37.0&new-version=1.38.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-31 16:44:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4674" class=".btn">#4674</a>
            </td>
            <td>
                <b>
                    chore: use temporary `displaydoc` fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Use the fix from https://github.com/yaahc/displaydoc/pull/47 until it is merged into the upstream.

### Linked issue

Closes #4567

### Benefits

Reduces warnings noise

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-31 04:50:03 +0000 UTC
    </div>
</div>

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
* New `kagami genesis sign` command to sign and transform `genesis.json` into `genesis.signed.scale` (SCALE serialized `SignedTransaction`)
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
                    fix: avoid early drop of `ConfigReader` in `iroha_client`
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

