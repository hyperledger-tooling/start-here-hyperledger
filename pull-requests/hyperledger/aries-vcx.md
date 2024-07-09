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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1260" class=".btn">#1260</a>
            </td>
            <td>
                <b>
                    Suppressed warnings and removed unused code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added #[allow(dead_code)]. on a few files to avoid building errors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 00:59:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1259" class=".btn">#1259</a>
            </td>
            <td>
                <b>
                    Update uniffi readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the new command for running the script should be: `sh aries/wrappers/uniffi-aries-vcx/scripts/android.build.cargo.ndk.sh`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 23:11:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1258" class=".btn">#1258</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde from 1.0.203 to 1.0.204 in /aries/misc/anoncreds_types
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
        Created At 2024-07-08 11:49:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1257" class=".btn">#1257</a>
            </td>
            <td>
                <b>
                    chore(deps): bump serde_json from 1.0.117 to 1.0.120 in /aries/misc/anoncreds_types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.117 to 1.0.120.
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
<h2>v1.0.118</h2>
<ul>
<li>Implement Hash for serde_json::Value (<a href="https://redirect.github.com/serde-rs/json/issues/1127">#1127</a>, thanks <a href="https://github.com/edwardycl"><code>@​edwardycl</code></a>)</li>
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
<li>Additional commits viewable in <a href="https://github.com/serde-rs/json/compare/v1.0.117...v1.0.120">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.117&new-version=1.0.120)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 11:49:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1256" class=".btn">#1256</a>
            </td>
            <td>
                <b>
                    chore(deps): bump clap from 4.5.6 to 4.5.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [clap](https://github.com/clap-rs/clap) from 4.5.6 to 4.5.8.
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
<h2>v4.5.7</h2>
<h2>[4.5.7] - 2024-06-10</h2>
<h3>Fixes</h3>
<ul>
<li>Clean up error message when too few arguments for <code>num_args</code></li>
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
<h2>[4.5.7] - 2024-06-10</h2>
<h3>Fixes</h3>
<ul>
<li>Clean up error message when too few arguments for <code>num_args</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/clap-rs/clap/commit/469d847d35731a987235d320517700c07ba729a4"><code>469d847</code></a> chore: Release</li>
<li><a href="https://github.com/clap-rs/clap/commit/e323b912a66d544f96deb2e0d868da7dc1f9ac36"><code>e323b91</code></a> docs: Update changelog</li>
<li><a href="https://github.com/clap-rs/clap/commit/7101c644f7daa9c664f75a2b1b5e1b67d7eb4ce5"><code>7101c64</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/5557">#5557</a> from tesuji/fish-positional-args-files</li>
<li><a href="https://github.com/clap-rs/clap/commit/5ee1a2570e5506972e57c42ebe42d6e1c0522abf"><code>5ee1a25</code></a> fix(fish): Don't ignore files if has positional args</li>
<li><a href="https://github.com/clap-rs/clap/commit/3a2fb2594793776583068f105c274716ba646187"><code>3a2fb25</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/5547">#5547</a> from tesuji/fish-list</li>
<li><a href="https://github.com/clap-rs/clap/commit/1e3681bfbcc896d9978c62095be410a29c6bbe89"><code>1e3681b</code></a> refactor: Pass list to __fish_seen_subcommand_from</li>
<li><a href="https://github.com/clap-rs/clap/commit/b1a0508cf926f04c1b73fab0e8ea2117d5a7be70"><code>b1a0508</code></a> refactor: Rewrite iterator for followup changes</li>
<li><a href="https://github.com/clap-rs/clap/commit/5cc44bb91ee3a13aad65a41fdf687fe7f30b8bdc"><code>5cc44bb</code></a> Merge pull request <a href="https://redirect.github.com/clap-rs/clap/issues/5548">#5548</a> from tesuji/fish-escape-tab</li>
<li><a href="https://github.com/clap-rs/clap/commit/181b9e0d9434a5aa7d9e9ef3bd76b3ad1a05d06f"><code>181b9e0</code></a> test: Ensure optional_value runs</li>
<li><a href="https://github.com/clap-rs/clap/commit/0724b7ba2b1d6de42a2647d747491b911fd07655"><code>0724b7b</code></a> chore: Remove tarpaulin support</li>
<li>Additional commits viewable in <a href="https://github.com/clap-rs/clap/compare/clap_complete-v4.5.6...v4.5.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clap&package-manager=cargo&previous-version=4.5.6&new-version=4.5.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 11:48:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1255" class=".btn">#1255</a>
            </td>
            <td>
                <b>
                    chore(deps): bump androidx.lifecycle:lifecycle-runtime-ktx from 2.3.1 to 2.8.3 in /aries/agents/mobile_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps androidx.lifecycle:lifecycle-runtime-ktx from 2.3.1 to 2.8.3.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=androidx.lifecycle:lifecycle-runtime-ktx&package-manager=gradle&previous-version=2.3.1&new-version=2.8.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 11:09:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1254" class=".btn">#1254</a>
            </td>
            <td>
                <b>
                    Handle trust pings in the AATH backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Close #1253 

This adds handling for TrustPing, which solves the issue of connections not entering complete state when VCX is the connection inviter.

# Results of ariesvcx-acapy manual runset of RFC0160
` behave -D Acme=http://0.0.0.0:9020 -D Bob=http://0.0.0.0:9030 -t @RFC0160 -t ~@wip -t ~@RFC0434 -t ~@RFC0453 -t ~@RFC0211 -t ~@DIDExchangeConnection -t ~@Transport_Ws`
## Before
all failures.

## After
(failures are due to running this with only 2 agents)
```
Failing scenarios:
  features/0160-connection.feature:52  Inviter Sends invitation for one agent second agent tries after connection
  features/0160-connection.feature:69  Inviter Sends invitation for one agent second agent tries during first share phase

0 features passed, 2 failed, 13 skipped
4 scenarios passed, 2 failed, 154 skipped
28 steps passed, 2 failed, 1353 skipped, 0 undefined
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-05 06:47:08 +0000 UTC
    </div>
</div>

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

