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
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Bump tokio from 1.21.2 to 1.24.2 in /rust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.21.2 to 1.24.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.24.1</h2>
<p>This release fixes a compilation failure on targets without <code>AtomicU64</code> when using rustc older than 1.63. (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5356">#5356</a>)</p>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5356">#5356</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5356">tokio-rs/tokio#5356</a></p>
<h2>Tokio v1.24.0</h2>
<p>The highlight of this release is the reduction of lock contention for all I/O operations (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5300">#5300</a>). We have received reports of up to a 20% improvement in CPU utilization and increased throughput for real-world I/O heavy applications.</p>
<h3>Fixed</h3>
<ul>
<li>rt: improve native <code>AtomicU64</code> support detection (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5284">#5284</a>)</li>
</ul>
<h3>Added</h3>
<ul>
<li>rt: add configuration option for max number of I/O events polled from the OS
per tick (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5186">#5186</a>)</li>
<li>rt: add an environment variable for configuring the default number of worker
threads per runtime instance (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4250">#4250</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>sync: reduce MPSC channel stack usage (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5294">#5294</a>)</li>
<li>io: reduce lock contention in I/O operations  (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5300">#5300</a>)</li>
<li>fs: speed up <code>read_dir()</code> by chunking operations (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5309">#5309</a>)</li>
<li>rt: use internal <code>ThreadId</code> implementation (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5329">#5329</a>)</li>
<li>test: don't auto-advance time when a <code>spawn_blocking</code> task is running (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5115">#5115</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5186">#5186</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5186">tokio-rs/tokio#5186</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5294">#5294</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5294">tokio-rs/tokio#5294</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5284">#5284</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5284">tokio-rs/tokio#5284</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4250">#4250</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4250">tokio-rs/tokio#4250</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5300">#5300</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5300">tokio-rs/tokio#5300</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5329">#5329</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5329">tokio-rs/tokio#5329</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5115">#5115</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5115">tokio-rs/tokio#5115</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5309">#5309</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5309">tokio-rs/tokio#5309</a></p>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/tokio-rs/tokio/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.21.2&new-version=1.24.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-02-04 00:43:56 +0000 UTC
    </div>
</div>

