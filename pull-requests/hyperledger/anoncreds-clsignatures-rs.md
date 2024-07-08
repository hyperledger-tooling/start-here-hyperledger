---
layout: default
title: anoncreds-clsignatures-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-clsignatures-rs
---

# anoncreds-clsignatures-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-clsignatures-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Bump serde_json from 1.0.119 to 1.0.120
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [serde_json](https://github.com/serde-rs/json) from 1.0.119 to 1.0.120.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/serde-rs/json/releases">serde_json's releases</a>.</em></p>
<blockquote>
<h2>v1.0.120</h2>
<ul>
<li>Correctly specify required version of <code>indexmap</code> dependency (<a href="https://redirect.github.com/serde-rs/json/issues/1152">#1152</a>, thanks <a href="https://github.com/cforycki"><code>@​cforycki</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/serde-rs/json/commit/bcedc3d96bcc33184f16d63eab397295e2193350"><code>bcedc3d</code></a> Release 1.0.120</li>
<li><a href="https://github.com/serde-rs/json/commit/962c0fbbecc7dc8559cfeb019c2611737512f937"><code>962c0fb</code></a> Merge pull request <a href="https://redirect.github.com/serde-rs/json/issues/1152">#1152</a> from cforycki/fix/index-map-minimal-version</li>
<li><a href="https://github.com/serde-rs/json/commit/3480feda7b572d33992544061a8e0fbf8610a803"><code>3480fed</code></a> fix: indexmap minimal version with Map::shift_insert()</li>
<li>See full diff in <a href="https://github.com/serde-rs/json/compare/v1.0.119...v1.0.120">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=serde_json&package-manager=cargo&previous-version=1.0.119&new-version=1.0.120)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-08 11:09:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-clsignatures-rs/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Bump serde from 1.0.203 to 1.0.204
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
        Created At 2024-07-08 11:09:19 +0000 UTC
    </div>
</div>

