---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1249" class=".btn">#1249</a>
            </td>
            <td>
                <b>
                    (refactor) small refactor to the new DIDExchange AnyXYZ wrappers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I started these changes mostly wanting to remove `Deserialize` trait from the `AnyXYZ` wrappers. As IMO trying to deserialize JSON back into AnyXYZ is dangerous; if both V1_0 & V1_1 variants are the same, then the serialized format is the same, so when deserializing `serde` cannot tell which variant it is, so it just picks the first one (misleading).

Also whilst i was here... i realised the Any wrappers were duplicating themselves alot, so i made a generic enum for it
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 00:56:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1248" class=".btn">#1248</a>
            </td>
            <td>
                <b>
                    chore(deps): bump uuid from 1.8.0 to 1.9.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [uuid](https://github.com/uuid-rs/uuid) from 1.8.0 to 1.9.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/uuid-rs/uuid/releases">uuid's releases</a>.</em></p>
<blockquote>
<h2>1.9.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Add an example of generating bulk v7 UUIDs by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/761">uuid-rs/uuid#761</a></li>
<li>Avoid taking the shared lock when getting usable bits in Uuid::now_v7 by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/762">uuid-rs/uuid#762</a></li>
<li>Prepare for 1.9.1 release by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/uuid-rs/uuid/pull/763">uuid-rs/uuid#763</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/uuid-rs/uuid/compare/1.9.0...1.9.1">https://github.com/uuid-rs/uuid/compare/1.9.0...1.9.1</a></p>
<h2>1.9.0</h2>
<h2><code>Uuid::now_v7()</code> is guaranteed to be monotonic</h2>
<p>Before this release, <code>Uuid::now_v7()</code> would only use the millisecond-precision timestamp for ordering. It now also uses a global 42-bit counter that's re-initialized each millisecond so that the following will always pass:</p>
<pre lang="rust"><code>let a = Uuid::now_v7();
let b = Uuid::now_v7();
<p>assert!(a &lt; b);<br />
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
<li><a href="https://github.com/uuid-rs/uuid/commit/36e6f573aa7b12a584cd4067de6ee6358794dd59"><code>36e6f57</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/763">#763</a> from uuid-rs/cargo/1.9.1</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/65bf733f83f659523fd61048e900e1bec94db0c3"><code>65bf733</code></a> prepare for 1.9.1 release</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/d0a24618ca4a0d7a96777ee3bbe184108f0e18cf"><code>d0a2461</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/762">#762</a> from uuid-rs/fix/double-lock</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/20911bddf50633aabc12162a2daf0294d5a7bc7a"><code>20911bd</code></a> avoid taking the shared lock when getting usable bits in Uuid::now_v7</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/c01feb813415ed050c0651d7f8875b019130ac75"><code>c01feb8</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/761">#761</a> from uuid-rs/chore/bulk-example</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/864239ba3005be222d9a6c7356d19c1622abd9fb"><code>864239b</code></a> add an example of generating bulk v7 UUIDs</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/4a129e728174a340ac2772f3cc6310ba77d1969f"><code>4a129e7</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/760">#760</a> from uuid-rs/cargo/1.9.0</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/6bfee6ba82ad8e7a0155f3161157dc3ea3a5d552"><code>6bfee6b</code></a> prepare for 1.9.0 release</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/62b7145d95913642298d5a954314ea28a199fa78"><code>62b7145</code></a> Merge pull request <a href="https://redirect.github.com/uuid-rs/uuid/issues/759">#759</a> from uuid-rs/chore/v7-counter-cleanup</li>
<li><a href="https://github.com/uuid-rs/uuid/commit/62e968c92b464c81a73b6002ab66a32c4bdad9ad"><code>62e968c</code></a> clean up new Timestamp APIs</li>
<li>Additional commits viewable in <a href="https://github.com/uuid-rs/uuid/compare/1.8.0...1.9.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=uuid&package-manager=cargo&previous-version=1.8.0&new-version=1.9.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 12:04:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1247" class=".btn">#1247</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_json from 1.0.117 to 1.0.119 in /aries/misc/anoncreds_types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.117 to 1.0.119.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.119</h2>
<ul>
<li>Add <code>serde_json::Map::shift_insert</code> (<a href="https://redirect.github.com/serde-rs/json/issues/1149">#1149</a>, thanks <a href="https://github.com/joshka"><code>@​joshka</code></a>)</li>
</ul>
<h2>v1.0.118</h2>
<ul>
<li>Implement Hash for serde_json::Value (<a href="https://redirect.github.com/serde-rs/json/issues/1127">#1127</a>, thanks <a href="https://github.com/edwardycl"><code>@​edwardycl</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/b48b9a3a0c09952579e98c8940fe0d1ee4aae588"><code>b48b9a3</code></a> Release 1.0.119</li>
<li><a href="https://github.com/serde-rs/json/commit/8878cd7c042a5f94ae4ee9889cbcbd12cc5ce334"><code>8878cd7</code></a> Make shift_insert available for inlining like other Map methods</li>
<li><a href="https://github.com/serde-rs/json/commit/352b7abf007cf3b9b063b01e0b1e8f6af62a4e39"><code>352b7ab</code></a> Document the cfg required for Map::shift_insert to exist</li>
<li><a href="https://github.com/serde-rs/json/commit/c17e63f6eff6cb40594beb1bddd4562c4cc81442"><code>c17e63f</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1149">#1149</a> from joshka/master</li>
<li><a href="https://github.com/serde-rs/json/commit/309ef6b8870e47622a283061cbda3f5514bfaf0d"><code>309ef6b</code></a> Add Map::shift_insert()</li>
<li><a href="https://github.com/serde-rs/json/commit/a9e089a2ce245bc223b56fbb6c525e2fe7b1f0ef"><code>a9e089a</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1146">#1146</a> from haouvw/master</li>
<li><a href="https://github.com/serde-rs/json/commit/a83fe96ae2a202925f1caa7abc51991f321d7c22"><code>a83fe96</code></a> chore: remove repeat words</li>
<li><a href="https://github.com/serde-rs/json/commit/c4f24f3be29a3d096d3ac7b1d5594777a613ec0d"><code>c4f24f3</code></a> Release 1.0.118</li>
<li><a href="https://github.com/serde-rs/json/commit/51d94ebdc07127de22fb655bdcf6a01d119492d5"><code>51d94eb</code></a> Combine Map's Hash into one impl</li>
<li><a href="https://github.com/serde-rs/json/commit/5e7bedc0a0e19ecda1c15a412ab7c69569f4aa84"><code>5e7bedc</code></a> Touch up PR 1127</li>
<li>Additional commits viewable in <a href="https://github.com/serde-rs/json/compare/v1.0.117...v1.0.119">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.117&new-version=1.0.119)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 11:18:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1246" class=".btn">#1246</a>
            </td>
            <td>
                <b>
                    chore(deps): bump log from 0.4.21 to 0.4.22 in /aries/misc/anoncreds_types
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
        Created At 2024-07-01 11:18:40 +0000 UTC
    </div>
</div>

