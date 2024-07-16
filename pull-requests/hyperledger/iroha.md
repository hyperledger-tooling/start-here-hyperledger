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
                PR <a href="https://github.com/hyperledger/iroha/pull/4850" class=".btn">#4850</a>
            </td>
            <td>
                <b>
                    refactor: reorganize project, fix Cargo issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

This fixes the error with `cargo install`:

```bash
package `.../client/tests/integration/smartcontracts/executor_custom_data_model/Cargo.toml` is a member of the wrong workspace
```

I'm not sure what exactly fixed it. It wasn't enough to just exclude it from the main `Cargo.toml`, maybe the additional unnesting did it.

- move all binary crates to `/bins`
- move all library crates to `/libs`
- move executors, smart contracts and triggers to `/samples`
- unnest `iroha_executor` and `iroha_trigger` from `iroha_smart_contract`
- rename crate directories to match their actual names (except nested utility crates)
- rename `configs` to `defaults`, remove `swarm` directory

### Linked issue

Closes #4293, #4320

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- binaries can be installed with `cargo install`
- separation between binaries and libraries
- more predictable structure and names

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
        Created At 2024-07-16 11:52:39 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4833" class=".btn">#4833</a>
            </td>
            <td>
                <b>
                    refactor: query filters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span>
            </td>
            <td>
                # Description

This PR introduces a lot of changes to the query subsystem. I tried to make the changes gradually in smaller PRs, but it ended up being very intertwined =(

## Summary of changes
- Queries are now split into two categories: iterable queries which return sequences of results and singular queries that return a single value. They are now fully disjoint traits stored in different Box enums, as they require very different handling.
- Query filters (aka predicates) are now typed depending on the type of the iterable query they are applied to (#4569). Instead of a single `PredicateBox` there is a predicate type for each queryable type (like `AccountPredicateBox`), with `CompountPredicate<T>` providing the logical operations on top.
- A new rust DSL to construct the predicates is introduced. It is designed to look very close to how one would write an `Iterator::filter` closure (`|obj| obj.field.inner_field.starts_with("hello")`) and is inspired by diesel's DSL.
- HTTP clients and wasm code (smart contracts, triggers and executor) are now using a common query builder struct, generic over a new `QueryExecutor` trait
- The HTTP API is majorly revamped to pass all of the params as scale-encoded values. This simplifies the torii handler, makes it more type-safe (can't add pagination to singular query) and allows sharing more code with wasm
- All of the queries that can be implemented as filtered versions of other queries are now removed. Here's a rough google table I made to keep track of all of them: https://docs.google.com/spreadsheets/d/1Cx9cU4wLk1ZyIa3Igx0NN9azl9dfqcXXMJMLKTMxes4/edit?usp=sharing

### The primary key question

Currently we have a bunch of queries that give you an object using its Primary Key (like `FindAccountById`). They can be implemented by filtering a basis query that returns all objects of such type (like `FindAllAccounts`). However, with naïve implementation (which this PR currently does) this would result in `O(n)` complexity instead of `O(log n)` that we currently have.

There is a way to do these lookups fast: just pattern-match the filter on the shape `|obj| obj.id.eq(expected_id)` and use the primary key index instead of linear scan. We can even use a similar approach to speed up other types of queries, if deemed necessary.

However, merging it as-is would mean that the primary queries would be slow. I can probably add the PK queries back for now, if that's unacceptable.

## Future work

These are improvements I see that can be made to this PR, but I would prefer them to be implemented in separate PRs. I'll convent them to issues when this PR gets closer to getting merged.

Perf:
- the Primary Key optimization (see above)
- make queries truly lazy (put them into the query store without collecting them all in a vec); Needs investigation whether that'll actually be beneficial and some clever implementation (need to store an iterator with lifetime tied to iroha state snapshot).

Ergonomics:
- `client::account::all()` is unfortunate, seeing as how most of the queries would be "all" with filters now
- provide helpers like `client::domain::by_id`, with them still relying on filtered queries
- `impl Into<String>` for ids (#4832)

Misc:
- `Display` representations for queries & filters (right now printing them with `Debug`)
- check that the iterable query continuation is executed by the same authority as the one that started it

## Linked issue

Closes #4569, #4720, #3720, #3671.

## Checklist

I still have a lot of doc strings, an overview of the predicate DSL implementation and some tests to write, hence marking this PR as a draft.

- [ ] add more docs and remove all the `#[warn(missing_docs)]`
- [ ] add more tests of the DSL
- [ ] add a test checking the validation performed on `SignedQueryCandidate`
- [ ] fix client cli tests
- [ ] fix ui tests
- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-10 17:29:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4831" class=".btn">#4831</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tomlkit from 0.12.5 to 0.13.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [tomlkit](https://github.com/sdispater/tomlkit) from 0.12.5 to 0.13.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-poetry/tomlkit/blob/master/CHANGELOG.md">tomlkit's changelog</a>.</em></p>
<blockquote>
<h2>[0.13.0] - 2024-07-10</h2>
<h3>Changed</h3>
<ul>
<li>Expect a tomlkit-specific error instead of <code>TypeError</code> from a custom encoder. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/355">#355</a>)</li>
<li>Drop support for Python older than 3.8. Remove 3.7 from the CI matrix.</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Fix the incompatiblity with 3.13 because of the <code>datetime.replace()</code> change. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/333">#333</a>)</li>
<li>Revert the change of parsing out-of-order tables. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/347">#347</a>)</li>
<li>Keep the nested out-of-order table. (<a href="https://redirect.github.com/python-poetry/tomlkit/issues/361">#361</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-poetry/tomlkit/commit/4d06dff4bc4a1cc16e0f600f71df8f41724efcec"><code>4d06dff</code></a> chore: bump version to 0.13.0</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/85aaf7a9231030fc3455048d78bfdabfe0a0a937"><code>85aaf7a</code></a> fix: keep the nested out of order table (<a href="https://redirect.github.com/sdispater/tomlkit/issues/366">#366</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/f12ece324fc376d0f863717005ba6acc5f9d8933"><code>f12ece3</code></a> chore(deps-dev): bump zipp from 3.15.0 to 3.19.1 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/365">#365</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/f4b2f74d2a4e19ee8bebd94b874c8c47699a169f"><code>f4b2f74</code></a> chore(deps-dev): bump requests from 2.31.0 to 2.32.2 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/364">#364</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/0747884431425b45071b696fd6ffe806d59304bb"><code>0747884</code></a> chore(deps-dev): bump urllib3 from 2.0.7 to 2.2.2 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/363">#363</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/d55d837d0b139bd48567ac90204baccb8ce0cbd9"><code>d55d837</code></a> fix: Remove 3.7 from the CI matrix</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/49daa69df84db37ab3e9ec365c3a9590d5455646"><code>49daa69</code></a> chore(deps-dev): bump certifi from 2024.2.2 to 2024.7.4 (<a href="https://redirect.github.com/sdispater/tomlkit/issues/362">#362</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/cce567ca4c1455d948d68c0fa32f7eb9196b9be3"><code>cce567c</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/sdispater/tomlkit/issues/359">#359</a>)</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/400057ba17dbf562fa4fe01fc26b40d7112690e4"><code>400057b</code></a> fix: <code>tomlkit</code> 0.12.5 : Encoder contract interferes with external <code>TypeError</code>...</li>
<li><a href="https://github.com/python-poetry/tomlkit/commit/22676f9a79228df216d79ba98209b98c2313c31c"><code>22676f9</code></a> Update tests action (<a href="https://redirect.github.com/sdispater/tomlkit/issues/357">#357</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/sdispater/tomlkit/compare/0.12.5...0.13.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tomlkit&package-manager=pip&previous-version=0.12.5&new-version=0.13.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-10 16:39:30 +0000 UTC
    </div>
</div>

