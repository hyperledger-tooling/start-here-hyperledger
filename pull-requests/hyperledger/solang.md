---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1595" class=".btn">#1595</a>
            </td>
            <td>
                <b>
                    Add a feature flag for the language server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The language server alone pulls over 200 dependencies, or close to half of our total dependencies. Currently, `cargo build` causes to compile 552 crates. With this feature flag, a `cargo build --no-default-features --features llvm,wasm_opt` compiles only 296 crates.

And there are some chunky ones in the language server too. With the LS I get the following timings:

|Rank| Unit | Total | Codegen | Features
|-- | -- | -- | -- | --
|1. | wasm-opt-sys v0.112.0 build script (run) | 50.1s |   |  
|2. | **ethers-solc v2.0.10** | 16.0s | 7.1s (45%) | async, futures-util, sha2, svm, svm-builds, svm-solc
|3. | solang v0.3.3 bin "solang" | 15.8s |   | contract-build, default, ethers-core, forge-fmt, inkwell,  language_server, libc, llvm, rust-lapper, tokio, tower-lsp, wasm-opt,  wasm_opt
|4. | solang-parser v0.3.3 build script (run) | 13.8s |   | default
|5. | solang-parser v0.3.2 build script (run) | 13.4s |   | default
|6. | **lsp-types v0.94.1** | 9.9s | 1.1s (11%) | default
|7. | **ethers-core v2.0.10** | 8.1s | 3.5s (43%) |  
|8. | lalrpop v0.20.0 | 7.9s | 3.1s (39%) |  
|9. | **tokio v1.34.0** | 7.1s | 3.6s (51%) | bytes, default, fs, io-std, io-util, libc, macros, mio, net,  num_cpus, process, rt, rt-multi-thread, signal-hook-registry, socket2,  sync, time, tokio-macros
|10. | solang v0.3.3 | 6.5s | 2.4s (38%) | contract-build, default, ethers-core, forge-fmt, inkwell,  language_server, libc, llvm, rust-lapper, tokio, tower-lsp, wasm-opt,  wasm_opt
|11. | syn v1.0.109 | 6.2s | 2.6s (41%) | clone-impls, default, derive, extra-traits, fold, full, parsing, printing, proc-macro, quote, visit, visit-mut
|12. | **foundry-config v0.2.0** | 6.2s | 4.1s (66%) | 


Main offender is still `wasm-opt` by far, but we already have a flag for this.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-14 10:25:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1594" class=".btn">#1594</a>
            </td>
            <td>
                <b>
                    Fix broken build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For some reason, cargo is not pick the latest version of ethers-core. This breaks the build. Add a line to Cargo.toml fixes the problem.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-14 09:27:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1593" class=".btn">#1593</a>
            </td>
            <td>
                <b>
                    Parse pragma solidity version numbers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Many Solidity features depend on the version of the compiler. So, parse the version pragma and in another PR we will use this information.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 16:32:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1592" class=".btn">#1592</a>
            </td>
            <td>
                <b>
                    Improve overloaded function call diagnostics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes: https://github.com/hyperledger/solang/issues/1534
Fixes: https://github.com/hyperledger/solang/issues/707
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 09:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1591" class=".btn">#1591</a>
            </td>
            <td>
                <b>
                    [Snyk] Upgrade @coral-xyz/anchor from 0.28.0 to 0.29.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to upgrade @coral-xyz/anchor from 0.28.0 to 0.29.0.</h3>

:information_source: Keep your dependencies up-to-date. This makes it easier to fix existing vulnerabilities and to more quickly identify and fix newly disclosed vulnerabilities when they affect your project.
<hr/>

- The recommended version is **3 versions** ahead of your current version.
- The recommended version was released **24 days ago**, on 2023-10-16.


<details>
<summary><b>Release notes</b></summary>
<br/>
  <details>
    <summary>Package name: <b>@coral-xyz/anchor</b></summary>
    <ul>
      <li>
        <b>0.29.0</b> - <a href="https://snyk.io/redirect/github/coral-xyz/anchor/releases/tag/v0.29.0">2023-10-16</a></br><p>Notable changes are listed in the <a href="https://snyk.io/redirect/github/coral-xyz/anchor/blob/v0.29.0/CHANGELOG.md#0290---2023-10-16">CHANGELOG</a>.</p>
<p>For this release, there is also <a href="https://snyk.io/redirect/github/coral-xyz/anchor/blob/v0.29.0/docs/src/pages/docs/release-notes.md">release notes</a> to get a better view on the changes.</p>
<p><a href="https://anchor-lang.com/docs/release-notes" rel="nofollow">https://anchor-lang.com/docs/release-notes</a></p>
      </li>
      <li>
        <b>0.28.1-beta.2</b> - 2023-08-27
      </li>
      <li>
        <b>0.28.1-beta.1</b> - 2023-06-21
      </li>
      <li>
        <b>0.28.0</b> - <a href="https://snyk.io/redirect/github/coral-xyz/anchor/releases/tag/v0.28.0">2023-06-09</a></br><p>For a list of changes in this release, see the <a href="https://snyk.io/redirect/github/coral-xyz/anchor/blob/master/CHANGELOG.md#0280---2023-06-09">Change Log</a>.</p>
      </li>
    </ul>
    from <a href="https://snyk.io/redirect/github/coral-xyz/anchor/releases">@coral-xyz/anchor GitHub release notes</a>
  </details>
</details>


<details>
  <summary><b>Commit messages</b></summary>
  </br>
  <details>
    <summary>Package name: <b>@coral-xyz/anchor</b></summary>
    <ul>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/fc9fd6d24b9be84abb2f40e47ed3faf7b11864ae">fc9fd6d</a> v0.29.0 (#2672)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/88a75aff138784fb99a7c9036b7c95b86f020bf0">88a75af</a> avm: Install from version-commit and refactor (#2671)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/4f996d0a58bd178a578a4e0d55952f48f8ec4ed2">4f996d0</a> cli: Add ability to override toolchain from &#x60;Anchor.toml&#x60; (#2649)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/5900c933102a06fbe7e5c4dedead883c807e35ce">5900c93</a> avm: Allow install, list and use from commit (#2659)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/8717364f81c106e61b3ab0a0bfe171b42efbee1e">8717364</a> Remove the maximum version constraint from Solana crates (#2667)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/23eeb1ec2d2d7e92f875f9cbfbc95bdec003a5a3">23eeb1e</a> spl: add feature memo to support cpi to spl-memo (#2661)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/0fef819e4bde38e7ff366266062a4b859c225d4a">0fef819</a> chore: Remove abusive cloning (#2663)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/6cf200493a307c01487c7b492b4893e0d6f6cb23">6cf2004</a> spl: Update dependencies to their latest versions (#2657)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/dcafb789e1635b8f90e8fd3badd0f9a015d204d4">dcafb78</a> lang: Add accounts by reference (#2656)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/243ab7573865a7296dd2af1153f44bffbf488458">243ab75</a> lang: Type safe bumps (#2542)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/721eb7a3be2344b2c5eae695ffe8eabf91fe7752">721eb7a</a> bench: Fix number formatting due to locale difference (#2655)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/267c4ceab7129c865680b0b9e7dd4376cc785265">267c4ce</a> tests: Remove &#x60;auction-house&#x60; submodule and host it natively (#2654)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/5e7fb445183f89abe79561d686785763eacb7a10">5e7fb44</a> Upgrade Solana to &#x60;1.17.0&#x60; (#2645)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/b0e725b5ace4bc3427a4e2c6350c1d6267176e23">b0e725b</a> spl: Update &#x60;mpl-token-metadata&#x60; to &#x60;3.1.0&#x60; and fix &#x60;create_metadata_accounts_v3&#x60; (#2651)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/25b24a1fd3fe7d411ec9f827b72d6167e6f55e56">25b24a1</a> syn: Fix having access to &#x60;idl&#x60; module by default (#2650)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/51578bcbc522d5398dbfa9d020f28fb797eb5815">51578bc</a> spl: Fix compilation error and warnings (#2647)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/5602244e1a3a3c2f9d7166d1114e2792aea4f0dc">5602244</a> cli: Support upgradeable program in anchor test (#2642)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/f18fd971fb10351bec268a4438ab3d6044506c07">f18fd97</a> Update Node to &#x60;18.18.0&#x60; LTS (#2643)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/e1d5e785b894d7a4ab4b06b21be2a9f4117df997">e1d5e78</a> syn: Fix generic type aliases (#2644)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/d1e32674d50005d04160b6fbac6f91de602a8829">d1e3267</a> Add type alias support (#2637)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/3e8bc76d72e2bfdb3962868b5066b2479cf49d25">3e8bc76</a> Update to solang v0.3.2 and add simple test (#2636)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/28adaf2343157835e546ffc8d0b3932eb1263427">28adaf2</a> ts: Remove &#x60;base64-js&#x60; dependency (#2635)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/99b75a905be2b407d4cd0a5f00c3db4cebd882e8">99b75a9</a> spl: Update to token metadata client sdk (#2632)</li>
      <li><a href="https://snyk.io/redirect/github/coral-xyz/anchor/commit/3c6fc2ba2d06a799b53b27a282e5c811b978cdf5">3c6fc2b</a> syn: Fix IDL named enum variant field being snake_case (#2633)</li>
    </ul>

   <a href="https://snyk.io/redirect/github/coral-xyz/anchor/compare/e1afcbf71e0f2e10fae14525934a6a68479167b9...fc9fd6d24b9be84abb2f40e47ed3faf7b11864ae">Compare</a>
  </details>
</details>
<hr/>

**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open upgrade PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiI0OWZhZjFiNC00ZGRkLTQyMmQtODhiOS0xNjI3M2UwOTk3OTYiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjQ5ZmFmMWI0LTRkZGQtNDIyZC04OGI5LTE2MjczZTA5OTc5NiJ9fQ==" width="0" height="0"/>

🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🛠 [Adjust upgrade PR settings](https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113/settings/integration?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr)

🔕 [Ignore this dependency or unsubscribe from future upgrade PRs](https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113/settings/integration?pkg&#x3D;@coral-xyz/anchor&amp;utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;upgrade-pr#auto-dep-upgrades)

<!--- (snyk:metadata:{"prId":"49faf1b4-4ddd-422d-88b9-16273e099796","prPublicId":"49faf1b4-4ddd-422d-88b9-16273e099796","dependencies":[{"name":"@coral-xyz/anchor","from":"0.28.0","to":"0.29.0"}],"packageManager":"npm","type":"auto","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/ccb2ab6a-ba20-4d58-979d-b59e66a8e113?utm_source=github&utm_medium=referral&page=upgrade-pr","projectPublicId":"ccb2ab6a-ba20-4d58-979d-b59e66a8e113","env":"prod","prType":"upgrade","vulns":[],"issuesToFix":[],"upgrade":[],"upgradeInfo":{"versionsDiff":3,"publishedDate":"2023-10-16T17:21:26.803Z"},"templateVariants":[],"hasFixes":false,"isMajorUpgrade":false,"isBreakingChange":false,"priorityScoreList":[]}) --->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 10:37:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1590" class=".btn">#1590</a>
            </td>
            <td>
                <b>
                    Implement string.concat() and bytes.concat()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is what solc implements. Solang has implement a + b for string concatenation, which this PR removes.

Fixes: https://github.com/hyperledger/solang/issues/1558
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 12:48:12 +0000 UTC
    </div>
</div>

