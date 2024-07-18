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
                PR <a href="https://github.com/hyperledger/iroha/pull/4863" class=".btn">#4863</a>
            </td>
            <td>
                <b>
                    fix: unnest wasm samples from `client`, exclude it from workspace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

- move `smartcontracts` out of `client/tests/integration`
- rename `smartcontracts` to `wasm_samples`
- pin `executor_custom_data_model` version in `client`
- exclude `wasm_samples` from the workspace
- move `default_executor` to `wasm_samples`

### Benefits

- fixes the error with `cargo install`:

  ```bash
  package `.../client/tests/integration/smartcontracts/executor_custom_data_model/Cargo.toml` 
  is a member of the wrong workspace
  ```

- wasm samples (executors, smartcontracts and triggers) are more discoverable
- Dependabot updates target all wasm samples instead of just the default executor

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
        Created At 2024-07-18 07:26:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4862" class=".btn">#4862</a>
            </td>
            <td>
                <b>
                    refactor: rename `configs` to `defaults`, remove `swarm`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Rename the `configs` directory to `defaults` since that's what it really is (default docker compose configs, default `executor.wasm`, default `genesis.json`, etc.)

### Linked issue

Closes #4293, #4320

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Conveys the purpose of the directory better.

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
        Created At 2024-07-18 06:37:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4860" class=".btn">#4860</a>
            </td>
            <td>
                <b>
                    ci: fix sonar dojo workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Removed lines that were bound to previous workflow.
<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
fixes this sonar_dojo [workflow](https://github.com/hyperledger/iroha/actions/runs/9978526258)
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
        Created At 2024-07-17 19:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4859" class=".btn">#4859</a>
            </td>
            <td>
                <b>
                    chore(deps): bump toml from 0.8.14 to 0.8.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [toml](https://github.com/toml-rs/toml) from 0.8.14 to 0.8.15.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/toml-rs/toml/commit/9217e44287880ce07777ae48fb8884a184957ae2"><code>9217e44</code></a> chore: Release</li>
<li><a href="https://github.com/toml-rs/toml/commit/003ce94f4c554e50cf81e4877874e699c7cf58c5"><code>003ce94</code></a> docs: Update changelog</li>
<li><a href="https://github.com/toml-rs/toml/commit/b463f3d7098d3680eec40e8c28d407d86b73d114"><code>b463f3d</code></a> Merge pull request <a href="https://redirect.github.com/toml-rs/toml/issues/757">#757</a> from epage/key</li>
<li><a href="https://github.com/toml-rs/toml/commit/3d8852b385576578a7462591f32250a919af31d0"><code>3d8852b</code></a> fix(encode): Be extra sure it can be a literal</li>
<li><a href="https://github.com/toml-rs/toml/commit/e1bc1c3861f208283c13410848dc34d73c1b0df4"><code>e1bc1c3</code></a> refactor(encode): Pull out literal inference</li>
<li><a href="https://github.com/toml-rs/toml/commit/fbb0ac28b5ddba66db2aef192ec6b269ea42079d"><code>fbb0ac2</code></a> test(encode): Add property-based tests for keys/strings</li>
<li><a href="https://github.com/toml-rs/toml/commit/0b268f20c11003de0fe2a886d15816fba41f4ed3"><code>0b268f2</code></a> fix(encode): Correct encoding for key with mixed quotes</li>
<li><a href="https://github.com/toml-rs/toml/commit/82c019557d77d4764f1128602d1b14d876d2e094"><code>82c0195</code></a> refactor(encode): Make str repr inferring clearer</li>
<li><a href="https://github.com/toml-rs/toml/commit/330b590968e00c94a6a9d4ee3cbb1f8615cf693c"><code>330b590</code></a> refactor(encode): Extract all str repr inferring</li>
<li><a href="https://github.com/toml-rs/toml/commit/00fb5eee54e9c8ee44860bc983753ff97e86a0da"><code>00fb5ee</code></a> test(edit): Add more roundtrip testing</li>
<li>Additional commits viewable in <a href="https://github.com/toml-rs/toml/compare/toml-v0.8.14...toml-v0.8.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=toml&package-manager=cargo&previous-version=0.8.14&new-version=0.8.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-17 16:59:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4858" class=".btn">#4858</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tokio from 1.38.0 to 1.38.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.38.0 to 1.38.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.38.1</h2>
<h1>1.38.1 (July 16th, 2024)</h1>
<p>This release fixes the bug identified as (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6682">#6682</a>), which caused timers not
to fire when they should.</p>
<h3>Fixed</h3>
<ul>
<li>time: update <code>wake_up</code> while holding all the locks of sharded time wheels (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6683">#6683</a>)</li>
</ul>
<p><a href="https://redirect.github.com/tokio-rs/tokio/issues/6682">#6682</a>: <a href="https://redirect.github.com/tokio-rs/tokio/pull/6682">tokio-rs/tokio#6682</a>
<a href="https://redirect.github.com/tokio-rs/tokio/issues/6683">#6683</a>: <a href="https://redirect.github.com/tokio-rs/tokio/pull/6683">tokio-rs/tokio#6683</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/14b9f7115728b77c82db8d21b6d768d16dc472a6"><code>14b9f71</code></a> chore: release Tokio v1.38.1 (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6688">#6688</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/24344dfe4b69931bfe9fe686d2424c9f626dc75b"><code>24344df</code></a> time: fix race condition leading to lost timers (<a href="https://redirect.github.com/tokio-rs/tokio/issues/6683">#6683</a>)</li>
<li>See full diff in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.38.0...tokio-1.38.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.38.0&new-version=1.38.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-17 16:40:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4857" class=".btn">#4857</a>
            </td>
            <td>
                <b>
                    refactor: replace `lol_alloc` with `dlmalloc`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Replaces `lol_alloc` with `dlmalloc`.
Check linked issue for more details.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4781 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

`dlmalloc` is used as default allocator for wasm in rust std lib, so we can expect it to be more stable

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
        Created At 2024-07-17 13:47:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4856" class=".btn">#4856</a>
            </td>
            <td>
                <b>
                    feat!: remove public key from ed25519 private key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Before ed25519 private key was represented as concatenation of private key and private key.
After the changes introduced in this PR it is just private key.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4838 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Private keys are more compact and doesn't contain unnecessary information.

### Downsides

Iroha environments have to be updated.

### For reviewers

All actual changes are in:
- [crypto/src/lib.rs](https://github.com/hyperledger/iroha/compare/main...Erigara:iroha:ed25519_private_key?expand=1#diff-b74424815b07b472bd526064fdd81233b3404546012d1c628228dc8ce5710100) serialization
- [crypto/src/signature/ed25519.rs](https://github.com/hyperledger/iroha/compare/main...Erigara:iroha:ed25519_private_key?expand=1#diff-8e5f1e972915bcea433b1892a54e9a4fce390aafcbedae989e9ccd9ad5f2f130) deserialization

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
        Created At 2024-07-17 11:11:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4855" class=".btn">#4855</a>
            </td>
            <td>
                <b>
                    fix(schema): rename `type_` to `type` in schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

* add support for handling `serde(rename)` attributes with `IntoSchema`
* attach `serde(rename = "type")` to `type_` fields in data model

### Linked issue

Closes #4770

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits



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
        Created At 2024-07-17 09:13:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4853" class=".btn">#4853</a>
            </td>
            <td>
                <b>
                    refactor: preserve voting block during block sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Refactor</span><span class="chip">Security</span>
            </td>
            <td>
                ## Description

This change allow to preserve voting block during block sync until iroha have to drop it to process transactions.

It is done in two ways: 
1. check block signatures before verification
2. try verify block without discarding voting block

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4834 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Preserve voting block in more cases.

### Downsides

Resulting code is not pretty.
Because it has to handle soft-fork case explicitly and not just revert previous block and proceed.

### How To Test

```
cargo test --package iroha_core --lib -- sumeragi::main_loop::tests::block_sync_commit_err_keep_voting_block --exact --show-output
```

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
        Created At 2024-07-16 14:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4852" class=".btn">#4852</a>
            </td>
            <td>
                <b>
                    fix: Fix `kagami genesis generate synthetic`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Fix account ids handling in `kagami genesis generate synthetic`

### Linked issue

Closes #4851

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
        Created At 2024-07-16 13:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4849" class=".btn">#4849</a>
            </td>
            <td>
                <b>
                    fix: Remove kura.lock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Originally `kura.lock` [was introduced](https://github.com/hyperledger/iroha/issues/3027) to prevent multiple iroha instances running with the same data directory. However if iroha doesn't remove `kura.lock`, e.g. in case of non-graceful shutdown, it causes problem that iroha couldn't start after restart. Also usually iroha is deployed using k8s cluster where each peer lives in different container so original problem is not relevant in this case. So it is proposed to remove `kura.lock`.

### Linked issue

Related: #4830
Related: #4848

### Benefits

Remove `kura.lock`, allowing Iroha to restart after non-graceful shutdown

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
        Created At 2024-07-16 11:12:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4847" class=".btn">#4847</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_with from 3.8.3 to 3.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_with](https://github.com/jonasbb/serde_with) from 3.8.3 to 3.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonasbb/serde_with/releases">serde_with's releases</a>.</em></p>
<blockquote>
<h2>serde_with v3.9.0</h2>
<h3>Added</h3>
<ul>
<li>
<p>Deserialize a map` and skip all elements failing to deserialize by <a href="https://github.com/johnmave126"><code>@​johnmave126</code></a> (<a href="https://redirect.github.com/jonasbb/serde_with/issues/763">#763</a>)</p>
<p><code>MapSkipError</code> acts like a map (<code>HashMap</code>/<code>BTreeMap</code>), but keys or values that fail to deserialize, like are ignored.</p>
<p>For formats with heterogeneously typed maps, we can collect only the elements where both key and value are deserializable.
This is also useful in conjunction to <code>#[serde(flatten)]</code> to ignore some entries when capturing additional fields.</p>
<pre lang="text"><code>// JSON
&quot;value&quot;: {&quot;0&quot;: &quot;v0&quot;, &quot;5&quot;: &quot;v5&quot;, &quot;str&quot;: &quot;str&quot;, &quot;10&quot;: 2},
<p>// Rust
#[serde_as(as = &quot;MapSkipError&lt;DisplayFromStr, _&gt;&quot;)]
value: BTreeMap&lt;u32, String&gt;,</p>
<p>// Only deserializes entries with a numerical key and a string value, i.e.,
{0 =&gt; &quot;v0&quot;, 5 =&gt; &quot;v5&quot;}
</code></pre></p>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonasbb/serde_with/commit/c3e489f4e571fadad9e656c28332b3708bd8cf0e"><code>c3e489f</code></a> Bump version to 3.9.0 (<a href="https://redirect.github.com/jonasbb/serde_with/issues/770">#770</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/57ad8778c46c0dd689002930430e3f994af1ebb1"><code>57ad877</code></a> Bump version to 3.9.0</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/d038657903639832437abcceca546395a0283034"><code>d038657</code></a> Implement <code>MapSkipError</code>, analogous to <code>VecSkipError</code>, but for map-like data ...</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/aaa0a2958917da51867ec90398d95826f8ebd717"><code>aaa0a29</code></a> Update serde_with/src/guide/serde_as_transformations.md</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/17dec1112b55bce9f7742ecf9d3414dcc089d26d"><code>17dec11</code></a> Add tests to make sure syntax errors are not suppressed.</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/97543d0c2d7588d9c2855c329bcc8c2b1107a404"><code>97543d0</code></a> Implement MapSkipError, skipping un-deserializable entries.</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/bf6724d2c09f35fb0ff917856829acf5362fed78"><code>bf6724d</code></a> Move VecSkipError to a separate file, preparing for MapSkipError</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/31e9172cabefd31b3cca12d24139e416e75ab6d8"><code>31e9172</code></a> Fix dead code warning by correcting a typo (<a href="https://redirect.github.com/jonasbb/serde_with/issues/769">#769</a>)</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/f5b2626307f7fb49275232a7f1925bfb5a200a37"><code>f5b2626</code></a> Fix dead code warnings in tests</li>
<li><a href="https://github.com/jonasbb/serde_with/commit/4ad4a1b4e9088219b7877d64aa225e6d352298e2"><code>4ad4a1b</code></a> Fix dead code warning by correcting a typo</li>
<li>See full diff in <a href="https://github.com/jonasbb/serde_with/compare/v3.8.3...v3.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_with&package-manager=cargo&previous-version=3.8.3&new-version=3.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-15 16:21:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4846" class=".btn">#4846</a>
            </td>
            <td>
                <b>
                    chore(deps): bump bytes from 1.6.0 to 1.6.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [bytes](https://github.com/tokio-rs/bytes) from 1.6.0 to 1.6.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/bytes/releases">bytes's releases</a>.</em></p>
<blockquote>
<h2>Bytes 1.6.1</h2>
<p>This release fixes a bug where <code>Bytes::is_unique</code> returns incorrect values when the <code>Bytes</code> originates from a shared <code>BytesMut</code>. (<a href="https://redirect.github.com/tokio-rs/bytes/issues/718">#718</a>)</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/bytes/blob/master/CHANGELOG.md">bytes's changelog</a>.</em></p>
<blockquote>
<h1>1.6.1 (July 13, 2024)</h1>
<p>This release fixes a bug where <code>Bytes::is_unique</code> returns incorrect values when
the <code>Bytes</code> originates from a shared <code>BytesMut</code>. (<a href="https://redirect.github.com/tokio-rs/bytes/issues/718">#718</a>)</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/bytes/commit/fd13c7dcdb840653bf81294d141da77d3f1f9e1f"><code>fd13c7d</code></a> chore: prepare bytes v1.6.1 (<a href="https://redirect.github.com/tokio-rs/bytes/issues/720">#720</a>)</li>
<li><a href="https://github.com/tokio-rs/bytes/commit/6b4b0eda2980f09df18380c80f8ae6109ae70d83"><code>6b4b0ed</code></a> Fix <code>Bytes::is_unique</code> when created from shared <code>BytesMut</code> (<a href="https://redirect.github.com/tokio-rs/bytes/issues/718">#718</a>)</li>
<li>See full diff in <a href="https://github.com/tokio-rs/bytes/compare/v1.6.0...v1.6.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=bytes&package-manager=cargo&previous-version=1.6.0&new-version=1.6.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-15 16:20:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4844" class=".btn">#4844</a>
            </td>
            <td>
                <b>
                    chore(deps): bump syn from 2.0.70 to 2.0.71
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [syn](https://github.com/dtolnay/syn) from 2.0.70 to 2.0.71.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/syn/releases">syn's releases</a>.</em></p>
<blockquote>
<h2>2.0.71</h2>
<ul>
<li>Do not require mutable borrow in Punctuated::get() (<a href="https://redirect.github.com/dtolnay/syn/issues/1706">#1706</a>, thanks <a href="https://github.com/lemunozm"><code>@​lemunozm</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/syn/commit/f34dc7bb53185a11f3aa45fc691488547c8c76ee"><code>f34dc7b</code></a> Release 2.0.71</li>
<li><a href="https://github.com/dtolnay/syn/commit/896d58bdb2508a089100247f01f7271222c518df"><code>896d58b</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/syn/issues/1706">#1706</a> from lemunozm/patch-1</li>
<li><a href="https://github.com/dtolnay/syn/commit/dd7e269f577dc33bcf92bec2583f7e53609081fb"><code>dd7e269</code></a> Remove mut from Puntuated::get()</li>
<li>See full diff in <a href="https://github.com/dtolnay/syn/compare/2.0.70...2.0.71">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=syn&package-manager=cargo&previous-version=2.0.70&new-version=2.0.71)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-12 16:15:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4843" class=".btn">#4843</a>
            </td>
            <td>
                <b>
                    chore(deps): bump thiserror from 1.0.61 to 1.0.62
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [thiserror](https://github.com/dtolnay/thiserror) from 1.0.61 to 1.0.62.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/thiserror/releases">thiserror's releases</a>.</em></p>
<blockquote>
<h2>1.0.62</h2>
<ul>
<li>Support referring to nested tuple struct fields inside <code>#[error(&quot;…&quot;, …)]</code> attribute (<a href="https://redirect.github.com/dtolnay/thiserror/issues/309">#309</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/thiserror/commit/0bf6e3dd781409b62cbcf0816ffa1bb970d24833"><code>0bf6e3d</code></a> Release 1.0.62</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/497793283934d9e514d903a14278af6babbfbb65"><code>4977932</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/thiserror/issues/310">#310</a> from dtolnay/nestedtuple</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/40a7779b1793f2dce5f85abe8c03486cdb5eb640"><code>40a7779</code></a> Support .0.0 nested tuple index</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/f1ca210cc4772f198af91886e3849dac68114f97"><code>f1ca210</code></a> Add regression test for issue 309</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/479744ec288f9183b8849f013dcee226ac6588ee"><code>479744e</code></a> No need for dead code if struct fields are public</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/4db08b10a39cfd189a36a88dee0fad578ac11cbe"><code>4db08b1</code></a> Ignore warning on unused struct in test</li>
<li><a href="https://github.com/dtolnay/thiserror/commit/f2824ae379ac2edee1fd687b9e56f18c048086cd"><code>f2824ae</code></a> Fill in ignore reasons in all #[ignore] attributes</li>
<li>See full diff in <a href="https://github.com/dtolnay/thiserror/compare/1.0.61...1.0.62">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=thiserror&package-manager=cargo&previous-version=1.0.61&new-version=1.0.62)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-12 16:14:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4841" class=".btn">#4841</a>
            </td>
            <td>
                <b>
                    fix: replace `Duration` with `u64` in schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

* replace `Duration` with `u64` in `schema.json`
* enable registering time trigger in genesis

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
        Created At 2024-07-12 11:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4837" class=".btn">#4837</a>
            </td>
            <td>
                <b>
                    feat(logger): use RUST_LOG-like EnvFilter for logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Replace level filter with `EnvFilter` which support setting specific log level for different iroha modules.

## Examples

The same can be done through configuration in config.toml.

```bash
# set global logging level to debug
LOG_LEVEL="debug" ./scripts/test_env.py setup
# set global logging level to error and info for iroha_core
LOG_LEVEL="error,iroha_core=info" ./scripts/test_env.py setup
# receive only logs from sumerag with trace level or heigher
LOG_LEVEL="iroha_core::sumeragi" ./scripts/test_env.py setup
# receive all logs at trace level, except axum for which use error
LOG_LEVEL="trace,axum=error" ./scripts/test_env.py setup
```

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4829 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

More granular control over logging.

### Downsides

It's harder to check correctness for example if someone would write `LOG_LEVEL=infa` iroha won't return any error because this would be parsed as accept logs from module `infa` at `trace` level.

I believe we can mitigate this, by custom parsing, but it would make our type more strict than orginal `EnvFilter`.
It's smt i would prefer to leave for separate PR.

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
        Created At 2024-07-11 14:34:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4836" class=".btn">#4836</a>
            </td>
            <td>
                <b>
                    fix(tests): correctly list asset definitions in CLI tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

* fix client cli pytests
* rename `--asset-id` to `--id` in client CLI
* add `asset definition` subparameter in CLI

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
        Created At 2024-07-11 13:31:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4835" class=".btn">#4835</a>
            </td>
            <td>
                <b>
                    ci: Move clippy and coverage tests jobs to PR workflow trigger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

- move clippy and coverage tests jobs to PR workflow trigger
- add workflow_run.id and trigger on completed for pushing artifacts produced in previous workflow 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->


<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- clippy and coverage tests will be made in one workflow with other tests
- artifacts can be pushed from separate workflow, making it possible to push test artifacts from forks

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
        Created At 2024-07-11 13:04:44 +0000 UTC
    </div>
</div>

