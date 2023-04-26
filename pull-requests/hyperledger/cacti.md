---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2403" class=".btn">#2403</a>
            </td>
            <td>
                <b>
                    feat(openssl): version upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …tements in cactus-plugin-keychain-vault package
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 03:20:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2402" class=".btn">#2402</a>
            </td>
            <td>
                <b>
                    chore(ci): revert to free runners
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
        Created At 2023-04-22 14:45:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2401" class=".btn">#2401</a>
            </td>
            <td>
                <b>
                    feat(driver): added Monitor to fabric driver for missed events and other fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. chore(testnet): upgrade fabric testnet to v2.5 in weaver and fix for mac
2. feat(driver): added Monitor to fabric driver for missed events
3. fix(weaversdk): ecies decrypt bug when z is less than 32Bytes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 19:12:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2400" class=".btn">#2400</a>
            </td>
            <td>
                <b>
                    build(deps): bump h2 from 0.3.12 to 0.3.18 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.12 to 0.3.18.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/releases">h2's releases</a>.</em></p>
<blockquote>
<h2>v0.3.18</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: pending-accept remotely-reset streams pattern was checking is_local by <a href="https://github.com/seanmonstar"><code>@​seanmonstar</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/676">hyperium/h2#676</a></li>
</ul>
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
<h2>v0.3.15</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove <code>B: Buf</code> bound on <code>SendStream</code>'s parameter by <a href="https://github.com/djkoloski"><code>@​djkoloski</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/614">hyperium/h2#614</a></li>
<li>add accessor for StreamId u32 by <a href="https://github.com/ehaydenr"><code>@​ehaydenr</code></a> in <a href="https://redirect.github.com/hyperium/h2/pull/639">hyperium/h2#639</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/ehaydenr"><code>@​ehaydenr</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/639">hyperium/h2#639</a></li>
</ul>
<h2>v0.3.14</h2>
<ul>
<li>Add <code>Error::is_reset</code> function.</li>
<li>Bump MSRV to Rust 1.56.</li>
<li>Return <code>RST_STREAM(NO_ERROR)</code> when the server early responds.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/djkoloski"><code>@​djkoloski</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/616">hyperium/h2#616</a></li>
<li><a href="https://github.com/bruceg"><code>@​bruceg</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/618">hyperium/h2#618</a></li>
<li><a href="https://github.com/ryanrussell"><code>@​ryanrussell</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/620">hyperium/h2#620</a></li>
<li><a href="https://github.com/kckeiks"><code>@​kckeiks</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/625">hyperium/h2#625</a></li>
<li><a href="https://github.com/erebe"><code>@​erebe</code></a> made their first contribution in <a href="https://redirect.github.com/hyperium/h2/pull/634">hyperium/h2#634</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/h2/blob/master/CHANGELOG.md">h2's changelog</a>.</em></p>
<blockquote>
<h1>0.3.18 (April 17, 2023)</h1>
<ul>
<li>Fix panic because of opposite check in <code>is_remote_local()</code>.</li>
</ul>
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
<h1>0.3.15 (October 21, 2022)</h1>
<ul>
<li>Remove <code>B: Buf</code> bound on <code>SendStream</code>'s parameter</li>
<li>add accessor for <code>StreamId</code> u32</li>
</ul>
<h1>0.3.14 (August 16, 2022)</h1>
<ul>
<li>Add <code>Error::is_reset</code> function.</li>
<li>Bump MSRV to Rust 1.56.</li>
<li>Return <code>RST_STREAM(NO_ERROR)</code> when the server early responds.</li>
</ul>
<h1>0.3.13 (March 31, 2022)</h1>
<ul>
<li>Update private internal <code>tokio-util</code> dependency.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/h2/commit/1b9f0704ff24d5f7939d16162082c5a764a0bfaa"><code>1b9f070</code></a> v0.3.18</li>
<li><a href="https://github.com/hyperium/h2/commit/1c6fa285afe436ca2a1f8abd38a6389353f360b6"><code>1c6fa28</code></a> fix: pending-accept remotely-reset streams pattern was checking is_local</li>
<li><a href="https://github.com/hyperium/h2/commit/af4bcacf6d3770e9e3dc10fdc631fc8c0bdd472b"><code>af4bcac</code></a> v0.3.17</li>
<li><a href="https://github.com/hyperium/h2/commit/d3f37e9fbad6608ba74419c355eb1892bd55d977"><code>d3f37e9</code></a> feat: add <code>max_pending_accept_reset_streams(n)</code> options</li>
<li><a href="https://github.com/hyperium/h2/commit/5bc8e72e5fcbd8ae2d3d9bc78a1c0ef0040bcc39"><code>5bc8e72</code></a> fix: limit the amount of pending-accept reset streams</li>
<li><a href="https://github.com/hyperium/h2/commit/8088ca658d90a3874fb6b136b85776424265295b"><code>8088ca6</code></a> feat: add Error::is_library method</li>
<li><a href="https://github.com/hyperium/h2/commit/481c31d5283bf32b90c83388c037494548934971"><code>481c31d</code></a> chore: Use Cargo metadata for the MSRV build job</li>
<li><a href="https://github.com/hyperium/h2/commit/d3d50ef8123f0a1b6d16faa2d9edc01418da7c00"><code>d3d50ef</code></a> chore: Replace unmaintained/outdated GitHub Actions</li>
<li><a href="https://github.com/hyperium/h2/commit/45b9bccdfcb26cfe9907123a1e975a22eb84c44f"><code>45b9bcc</code></a> chore: set rust-version in Cargo.toml (<a href="https://redirect.github.com/hyperium/h2/issues/664">#664</a>)</li>
<li><a href="https://github.com/hyperium/h2/commit/b9dcd39915420ab1d9f4a8ad0f96c86af8f86558"><code>b9dcd39</code></a> v0.3.16</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/h2/compare/v0.3.12...v0.3.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.12&new-version=0.3.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 11:15:00 +0000 UTC
    </div>
</div>

