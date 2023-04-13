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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/803" class=".btn">#803</a>
            </td>
            <td>
                <b>
                    Bump h2 from 0.3.15 to 0.3.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.15 to 0.3.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/releases">h2's releases</a>.</em></p>
<blockquote>
<h2>v0.3.17</h2>
<h2>What's Changed</h2>
<ul>
<li>Add <code>Error::is_library()</code> method to check if the originated inside <code>h2</code>.</li>
<li>Add <code>max_pending_accept_reset_streams(usize)</code> option to client and server
builders.</li>
<li>Fix theoretical memory growth when receiving too many HEADERS and then
RST_STREAM frames faster than an application can accept them off the queue.
(CVE-2023-26964)</li>
</ul>
<h2>v0.3.16</h2>
<h2>What's Changed</h2>
<ul>
<li>Set <code>Protocol</code> extension on requests when received Extended CONNECT requests.</li>
<li>Remove <code>B: Unpin + 'static</code> bound requiremented of bufs</li>
<li>Fix releasing of frames when stream is finished, reducing memory usage.</li>
<li>Fix panic when trying to send data and connection window is available, but stream window is not.</li>
<li>Fix spurious wakeups when stream capacity is not available.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vi"><code>@​vi</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/646">hyperium/h2#646</a></li>
<li><a href="https://github.com/silence-coding"><code>@​silence-coding</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/651">hyperium/h2#651</a></li>
<li><a href="https://github.com/gtsiam"><code>@​gtsiam</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/649">hyperium/h2#649</a></li>
<li><a href="https://github.com/howardjohn"><code>@​howardjohn</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/658">hyperium/h2#658</a></li>
<li><a href="https://github.com/cloneable"><code>@​cloneable</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/655">hyperium/h2#655</a></li>
<li><a href="https://github.com/aftersnow"><code>@​aftersnow</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/657">hyperium/h2#657</a></li>
<li><a href="https://github.com/vadim-eg"><code>@​vadim-eg</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/661">hyperium/h2#661</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/blob/master/CHANGELOG.md">h2's changelog</a>.</em></p>
<blockquote>
<h1>0.3.17 (April 13, 2023)</h1>
<ul>
<li>Add <code>Error::is_library()</code> method to check if the originated inside <code>h2</code>.</li>
<li>Add <code>max_pending_accept_reset_streams(usize)</code> option to client and server
builders.</li>
<li>Fix theoretical memory growth when receiving too many HEADERS and then
RST_STREAM frames faster than an application can accept them off the queue.
(CVE-2023-26964)</li>
</ul>
<h1>0.3.16 (February 27, 2023)</h1>
<ul>
<li>Set <code>Protocol</code> extension on requests when received Extended CONNECT requests.</li>
<li>Remove <code>B: Unpin + 'static</code> bound requiremented of bufs</li>
<li>Fix releasing of frames when stream is finished, reducing memory usage.</li>
<li>Fix panic when trying to send data and connection window is available, but stream window is not.</li>
<li>Fix spurious wakeups when stream capacity is not available.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/h2/commit/af4bcacf6d3770e9e3dc10fdc631fc8c0bdd472b"><code>af4bcac</code></a> v0.3.17</li>
<li><a href="https://github.com/hyperium/h2/commit/d3f37e9fbad6608ba74419c355eb1892bd55d977"><code>d3f37e9</code></a> feat: add <code>max_pending_accept_reset_streams(n)</code> options</li>
<li><a href="https://github.com/hyperium/h2/commit/5bc8e72e5fcbd8ae2d3d9bc78a1c0ef0040bcc39"><code>5bc8e72</code></a> fix: limit the amount of pending-accept reset streams</li>
<li><a href="https://github.com/hyperium/h2/commit/8088ca658d90a3874fb6b136b85776424265295b"><code>8088ca6</code></a> feat: add Error::is_library method</li>
<li><a href="https://github.com/hyperium/h2/commit/481c31d5283bf32b90c83388c037494548934971"><code>481c31d</code></a> chore: Use Cargo metadata for the MSRV build job</li>
<li><a href="https://github.com/hyperium/h2/commit/d3d50ef8123f0a1b6d16faa2d9edc01418da7c00"><code>d3d50ef</code></a> chore: Replace unmaintained/outdated GitHub Actions</li>
<li><a href="https://github.com/hyperium/h2/commit/45b9bccdfcb26cfe9907123a1e975a22eb84c44f"><code>45b9bcc</code></a> chore: set rust-version in Cargo.toml (<a href="https://redirect.github.com/hyperium/h2/issues/664">#664</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/b9dcd39915420ab1d9f4a8ad0f96c86af8f86558"><code>b9dcd39</code></a> v0.3.16</li>
<li><a href="https://github.com/hyperium/h2/commit/96caf4fca32fad92037e082b6b74220274faaf16"><code>96caf4f</code></a> Add a message for EOF-related broken pipe errors (<a href="https://redirect.github.com/hyperium/h2/issues/615">#615</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/732319039ff6184076b339f6870746b6c7fed86f"><code>7323190</code></a> Avoid spurious wakeups when stream capacity is not available (<a href="https://redirect.github.com/hyperium/h2/issues/661">#661</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/h2/compare/v0.3.15...v0.3.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.15&new-version=0.3.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-vcx/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 17:05:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/802" class=".btn">#802</a>
            </td>
            <td>
                <b>
                    Release 0.54.0
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
        Created At 2023-04-13 07:20:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/801" class=".btn">#801</a>
            </td>
            <td>
                <b>
                    post_message migration [Issue #772]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **  Still working on getting the tests passing :)  **

Resolves: Issue https://github.com/hyperledger/aries-vcx/issues/772 - Move out post_message to shared_vcx

**Short Summary**

- Migrated httpclient.rs file to shared_vcx directory
- The issue requested that the post_message() function be moved, but there were other items within httpclient.rs that post_message() depended upon.
- aries-vcx is successfully compiling with the changes provided.

Note: This is a new branch created from the work previously pushed to my fork's main (which has since been reset to sync w/ aries-vcx upstream repo).

Old PR: https://github.com/hyperledger/aries-vcx/pull/790
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 20:00:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/800" class=".btn">#800</a>
            </td>
            <td>
                <b>
                    Bump time to `0.3.20`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses the breaking changes in the `time` crate dependency.  
This PR aims to upgrade `time` to `0.3.20`.  
Fixes #795 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 17:26:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/798" class=".btn">#798</a>
            </td>
            <td>
                <b>
                    Separate core into a standalone crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Relocates `BaseLedger`,` BaseAnonCreds`, `BaseWallet` trait definitions and their corresponding implementations (including the `indy` module and related `utils`) into a distinct crate called `aries_vcx_core`. As a result, `aries-vcx` now depends on `indy-vdr`, `indy-credx`, and  `libvdrtools` indirectly through this new crate, which doesn't reexport any of them.

The primary objective of this pull request is the separation of these components, and no additional efforts were made to enhance the codebase beyond this specific aim.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 17:18:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/797" class=".btn">#797</a>
            </td>
            <td>
                <b>
                    Remove deps in `aries-vcx`: `env_logger`, `android_logger`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - `aries-vcx` should not specify `log` implementation, removed `env_logger` as well as android build dependency `android_logger`
- similar changes in other crates as well
- added `env_logger` to `vcx-napi-rs` along with its initialization (same as previously in `aries-vcx`) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 07:41:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    Remove unnecessary dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed unused dependencies across the board
- `vdrtools`: Remove unused ffi wallet declarations (in `libvdrtools/indy-api-types/src/lib.rs`) and unsupported function for wallet plugin registration `register_wallet_storage`
- Removed commented tests in vdrtools
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 20:13:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/794" class=".btn">#794</a>
            </td>
            <td>
                <b>
                    Remove proof verifier legacy format deserialization support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - As planned in https://github.com/hyperledger/aries-vcx/pull/770 next release won't support legacy format of serialized verifier proofs. 

- Follow migration guide in the PR linked above using aries-vcx `0.53.0` to reserialize your verifier proofs to the new format. The next `aries-vcx` release `0.54.0` will not support non-migrated verifier proofs created by `aries-vcx` `0.52.x` or older.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 17:41:17 +0000 UTC
    </div>
</div>

