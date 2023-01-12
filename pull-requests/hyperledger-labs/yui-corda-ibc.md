---
layout: default
title: yui-corda-ibc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-corda-ibc
---

# yui-corda-ibc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-corda-ibc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Pluggable App Module Support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #45 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-12 16:36:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Bump tokio from 1.21.2 to 1.23.1 in /rust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.21.2 to 1.23.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.23.1</h2>
<p>This release forward ports changes from 1.18.4.</p>
<h3>Fixed</h3>
<ul>
<li>net: fix Windows named pipe server builder to maintain option when toggling
pipe mode (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5336">#5336</a>).</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5336">#5336</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5336">tokio-rs/tokio#5336</a></p>
<h2>Tokio v1.23.0</h2>
<h3>Fixed</h3>
<ul>
<li>net: fix Windows named pipe connect (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5208">#5208</a>)</li>
<li>io: support vectored writes for <code>ChildStdin</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5216">#5216</a>)</li>
<li>io: fix <code>async fn ready()</code> false positive for OS-specific events (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5231">#5231</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>runtime: <code>yield_now</code> defers task until after driver poll (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5223">#5223</a>)</li>
<li>runtime: reduce amount of codegen needed per spawned task (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5213">#5213</a>)</li>
<li>windows: replace <code>winapi</code> dependency with <code>windows-sys</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5204">#5204</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5208">#5208</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5208">tokio-rs/tokio#5208</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5216">#5216</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5216">tokio-rs/tokio#5216</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5213">#5213</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5213">tokio-rs/tokio#5213</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5204">#5204</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5204">tokio-rs/tokio#5204</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5223">#5223</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5223">tokio-rs/tokio#5223</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5231">#5231</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5231">tokio-rs/tokio#5231</a></p>
<h2>Tokio v1.22.0</h2>
<h3>Added</h3>
<ul>
<li>runtime: add <code>Handle::runtime_flavor</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5138">#5138</a>)</li>
<li>sync: add <code>Mutex::blocking_lock_owned</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5130">#5130</a>)</li>
<li>sync: add <code>Semaphore::MAX_PERMITS</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5144">#5144</a>)</li>
<li>sync: add <code>merge()</code> to semaphore permits (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4948">#4948</a>)</li>
<li>sync: add <code>mpsc::WeakUnboundedSender</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5189">#5189</a>)</li>
</ul>
<h3>Added (unstable)</h3>
<ul>
<li>process: add <code>Command::process_group</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5114">#5114</a>)</li>
<li>runtime: export metrics about the blocking thread pool (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5161">#5161</a>)</li>
<li>task: add <code>task::id()</code> and <code>task::try_id()</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5171">#5171</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>macros: don't take ownership of futures in macros (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5087">#5087</a>)</li>
<li>runtime: fix Stacked Borrows violation in <code>LocalOwnedTasks</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5099">#5099</a>)</li>
<li>runtime: mitigate ABA with 32-bit queue indices when possible (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5042">#5042</a>)</li>
<li>task: wake local tasks to the local queue when woken by the same thread (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5095">#5095</a>)</li>
<li>time: panic in release mode when <code>mark_pending</code> called illegally (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5093">#5093</a>)</li>
<li>runtime: fix typo in expect message (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5169">#5169</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/1a997ffbd62334af2553775234e75ede2d7d949f"><code>1a997ff</code></a> chore: prepare Tokio v1.23.1 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/a8fe333cc45c14b0566d450dff8ff85fbe974fa0"><code>a8fe333</code></a> Merge branch 'tokio-1.20.x' into tokio-1.23.x</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/ba81945ffc2695b71f2bbcadbfb5e46ec55aaef3"><code>ba81945</code></a> chore: prepare Tokio 1.20.3 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/763bdc967e3e128d1e6e000238f1d257a81bf59a"><code>763bdc9</code></a> ci: run WASI tasks using latest Rust</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9f98535877f8f706b436447952f40f153e2a52dc"><code>9f98535</code></a> Merge remote-tracking branch 'origin/tokio-1.18.x' into fix-named-pipes-1.20</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9241c3eddf4a6a218681b088d71f7191513e2376"><code>9241c3e</code></a> chore: prepare Tokio v1.18.4 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/699573d550fabf4bfb45d82505d6709faaae9037"><code>699573d</code></a> net: fix named pipes server configuration builder</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/3ce5a2681c734e134c2aa6d6cf91b8d2631bd82b"><code>3ce5a26</code></a> chore: prepare Tokio v1.23 release (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5270">#5270</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/644cb8207df09c19543cf9b096a43a66f8df9a0f"><code>644cb82</code></a> rt: fix <code>*_closed</code> false positives (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5231">#5231</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/a1316cd792596baa079144bf4672f59e99556531"><code>a1316cd</code></a> io: impl <code>std::io::BufRead</code> on <code>SyncIoBridge\&lt;T&gt;</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5265">#5265</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.21.2...tokio-1.23.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.21.2&new-version=1.23.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-corda-ibc/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 21:52:15 +0000 UTC
    </div>
</div>

