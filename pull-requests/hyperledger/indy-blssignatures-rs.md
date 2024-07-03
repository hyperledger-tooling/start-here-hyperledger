---
layout: default
title: indy-blssignatures-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-blssignatures-rs
---

# indy-blssignatures-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-blssignatures-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-blssignatures-rs/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Bump log from 0.4.19 to 0.4.22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [log](https://github.com/rust-lang/log) from 0.4.19 to 0.4.22.
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
<h2>[0.4.21] - 2024-02-27</h2>
<h2>What's Changed</h2>
<ul>
<li>Minor clippy nits by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/578">rust-lang/log#578</a></li>
<li>Simplify Display impl by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/579">rust-lang/log#579</a></li>
<li>Set all crates to 2021 edition by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/580">rust-lang/log#580</a></li>
<li>Various changes based on review by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/583">rust-lang/log#583</a></li>
<li>Fix typo in file_static() method doc by <a href="https://github.com/dimo414"><code>@​dimo414</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/590">rust-lang/log#590</a></li>
<li>Specialize empty key value pairs by <a href="https://github.com/EFanZh"><code>@​EFanZh</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/576">rust-lang/log#576</a></li>
<li>Fix incorrect lifetime in Value::to_str() by <a href="https://github.com/peterjoel"><code>@​peterjoel</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/587">rust-lang/log#587</a></li>
<li>Remove some API of the key-value feature by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/585">rust-lang/log#585</a></li>
<li>Add logcontrol-log and log-reload by <a href="https://github.com/swsnr"><code>@​swsnr</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/595">rust-lang/log#595</a></li>
<li>Add Serialization section to kv::Value docs by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/593">rust-lang/log#593</a></li>
<li>Rename Value::to_str to to_cow_str by <a href="https://github.com/Thomasdezeeuw"><code>@​Thomasdezeeuw</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/592">rust-lang/log#592</a></li>
<li>Clarify documentation and simplify initialization of <code>STATIC_MAX_LEVEL</code> by <a href="https://github.com/ptosi"><code>@​ptosi</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/594">rust-lang/log#594</a></li>
<li>Update docs to 2021 edition, test by <a href="https://github.com/nyurik"><code>@​nyurik</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/577">rust-lang/log#577</a></li>
<li>Add &quot;alterable_logger&quot; link to README.md by <a href="https://github.com/brummer-simon"><code>@​brummer-simon</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/589">rust-lang/log#589</a></li>
<li>Normalize line ending by <a href="https://github.com/EFanZh"><code>@​EFanZh</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/602">rust-lang/log#602</a></li>
<li>Remove <code>ok_or</code> in favor of <code>Option::ok_or</code> by <a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/607">rust-lang/log#607</a></li>
<li>Use <code>Acquire</code> ordering for initialization check by <a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/610">rust-lang/log#610</a></li>
<li>Get structured logging API ready for stabilization by <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a> in <a href="https://redirect.github.com/rust-lang/log/pull/613">rust-lang/log#613</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/nyurik"><code>@​nyurik</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/578">rust-lang/log#578</a></li>
<li><a href="https://github.com/dimo414"><code>@​dimo414</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/590">rust-lang/log#590</a></li>
<li><a href="https://github.com/peterjoel"><code>@​peterjoel</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/587">rust-lang/log#587</a></li>
<li><a href="https://github.com/ptosi"><code>@​ptosi</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/594">rust-lang/log#594</a></li>
<li><a href="https://github.com/brummer-simon"><code>@​brummer-simon</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/589">rust-lang/log#589</a></li>
<li><a href="https://github.com/AngelicosPhosphoros"><code>@​AngelicosPhosphoros</code></a> made their first contribution in <a href="https://redirect.github.com/rust-lang/log/pull/607">rust-lang/log#607</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
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
<li>Additional commits viewable in <a href="https://github.com/rust-lang/log/compare/0.4.19...0.4.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=log&package-manager=cargo&previous-version=0.4.19&new-version=0.4.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 11:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-blssignatures-rs/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Bump serde_json from 1.0.104 to 1.0.119
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.104 to 1.0.119.
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
<h2>v1.0.117</h2>
<ul>
<li>Resolve unexpected_cfgs warning (<a href="https://redirect.github.com/serde-rs/json/issues/1130">#1130</a>)</li>
</ul>
<h2>v1.0.116</h2>
<ul>
<li>Make module structure comprehensible to static analysis (<a href="https://redirect.github.com/serde-rs/json/issues/1124">#1124</a>, thanks <a href="https://github.com/mleonhard"><code>@​mleonhard</code></a>)</li>
</ul>
<h2>v1.0.115</h2>
<ul>
<li>Documentation improvements</li>
</ul>
<h2>v1.0.114</h2>
<ul>
<li>Fix unused_imports warnings when compiled by rustc 1.78</li>
</ul>
<h2>v1.0.113</h2>
<ul>
<li>Add <code>swap_remove</code> and <code>shift_remove</code> methods on Map (<a href="https://redirect.github.com/serde-rs/json/issues/1109">#1109</a>)</li>
</ul>
<h2>v1.0.112</h2>
<ul>
<li>Improve formatting of &quot;invalid type&quot; error messages involving floats (<a href="https://redirect.github.com/serde-rs/json/issues/1107">#1107</a>)</li>
</ul>
<h2>v1.0.111</h2>
<ul>
<li>Improve floating point parsing performance on loongarch64 (<a href="https://redirect.github.com/serde-rs/json/issues/1100">#1100</a>, thanks <a href="https://github.com/heiher"><code>@​heiher</code></a>)</li>
</ul>
<h2>v1.0.110</h2>
<ul>
<li>Update proc-macro2 to fix caching issue when using a rustc-wrapper such as sccache</li>
</ul>
<h2>v1.0.109</h2>
<ul>
<li>Documentation improvements</li>
</ul>
<h2>v1.0.108</h2>
<ul>
<li>Documentation improvements (<a href="https://redirect.github.com/serde-rs/json/issues/1075">#1075</a>, <a href="https://redirect.github.com/serde-rs/json/issues/1081">#1081</a>, <a href="https://redirect.github.com/serde-rs/json/issues/1082">#1082</a>, thanks <a href="https://github.com/dimo414"><code>@​dimo414</code></a> and <a href="https://github.com/fritzrehde"><code>@​fritzrehde</code></a>)</li>
</ul>
<h2>v1.0.107</h2>
<ul>
<li>impl IntoDeserializer for &amp;RawValue (<a href="https://redirect.github.com/serde-rs/json/issues/1071">#1071</a>)</li>
</ul>
<h2>v1.0.106</h2>
<ul>
<li>Add <code>Value::as_number</code> accessor (<a href="https://redirect.github.com/serde-rs/json/issues/1069">#1069</a>, thanks <a href="https://github.com/chanced"><code>@​chanced</code></a>)</li>
<li>Add <code>Number::as_str</code> accessor under &quot;arbitrary_precision&quot; feature (<a href="https://redirect.github.com/serde-rs/json/issues/1067">#1067</a>, thanks <a href="https://github.com/chanced"><code>@​chanced</code></a>)</li>
</ul>
<h2>v1.0.105</h2>
<ul>
<li>Support bool in map keys (<a href="https://redirect.github.com/serde-rs/json/issues/1054">#1054</a>)</li>
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
<li>Additional commits viewable in <a href="https://github.com/serde-rs/json/compare/v1.0.104...v1.0.119">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.104&new-version=1.0.119)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-01 11:15:45 +0000 UTC
    </div>
</div>

