---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2247" class=".btn">#2247</a>
            </td>
            <td>
                <b>
                    build(deps): bump tokio from 1.19.2 to 1.20.3 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.19.2 to 1.20.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.20.2</h2>
<h1>1.20.2 (September 27, 2022)</h1>
<p>This release removes the dependency on the <code>once_cell</code> crate to restore the MSRV of the 1.20.x LTS release. (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>)</p>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/5048">tokio-rs/tokio#5048</a></p>
<h2>Tokio v1.20.1</h2>
<h1>1.20.1 (July 25, 2022)</h1>
<h3>Fixed</h3>
<ul>
<li>chore: fix version detection in build script (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4860">#4860</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4860">#4860</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4860">tokio-rs/tokio#4860</a></p>
<h2>Tokio v1.20.0</h2>
<h1>1.20.0 (July 12, 2022)</h1>
<h3>Added</h3>
<ul>
<li>tokio: add track_caller to public APIs (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4772">#4772</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4791">#4791</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4793">#4793</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4806">#4806</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4808">#4808</a>)</li>
<li>sync: Add <code>has_changed</code> method to <code>watch::Ref</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4758">#4758</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>time: remove <code>src/time/driver/wheel/stack.rs</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4766">#4766</a>)</li>
<li>rt: clean up arguments passed to basic scheduler (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4767">#4767</a>)</li>
<li>net: be more specific about winapi features (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4764">#4764</a>)</li>
<li>tokio: use const initialized thread locals where possible (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4677">#4677</a>)</li>
<li>task: various small improvements to LocalKey (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4795">#4795</a>)</li>
</ul>
<h3>Fixed</h3>
<h3>Documented</h3>
<ul>
<li>fs: warn about performance pitfall (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4762">#4762</a>)</li>
<li>chore: fix spelling (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4769">#4769</a>)</li>
<li>sync: document spurious failures in oneshot (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4777">#4777</a>)</li>
<li>sync: add warning for watch in non-Send futures (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4741">#4741</a>)</li>
<li>chore: fix typo (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4798">#4798</a>)</li>
</ul>
<h3>Unstable</h3>
<ul>
<li>joinset: rename <code>join_one</code> to <code>join_next</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4755">#4755</a>)</li>
<li>rt: unhandled panic config for current thread rt (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4770">#4770</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4677">#4677</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4677">tokio-rs/tokio#4677</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4741">#4741</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4741">tokio-rs/tokio#4741</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4755">#4755</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4755">tokio-rs/tokio#4755</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4758">#4758</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4758">tokio-rs/tokio#4758</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4762">#4762</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/4762">tokio-rs/tokio#4762</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/ba81945ffc2695b71f2bbcadbfb5e46ec55aaef3"><code>ba81945</code></a> chore: prepare Tokio 1.20.3 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/763bdc967e3e128d1e6e000238f1d257a81bf59a"><code>763bdc9</code></a> ci: run WASI tasks using latest Rust</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9f98535877f8f706b436447952f40f153e2a52dc"><code>9f98535</code></a> Merge remote-tracking branch 'origin/tokio-1.18.x' into fix-named-pipes-1.20</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9241c3eddf4a6a218681b088d71f7191513e2376"><code>9241c3e</code></a> chore: prepare Tokio v1.18.4 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/699573d550fabf4bfb45d82505d6709faaae9037"><code>699573d</code></a> net: fix named pipes server configuration builder</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/3d95a4626fc136b55e82e6bd480e14459a77a22c"><code>3d95a46</code></a> chore: prepare Tokio v1.20.2 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5055">#5055</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/2063d6692e1a2f12522299d2e6f16dd482ebbb05"><code>2063d66</code></a> Merge 'tokio-1.18.3' into 'tokio-1.20.x' (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5054">#5054</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/5c76d070e28bd9153ec72f13d0ebe24935b9dea0"><code>5c76d07</code></a> chore: prepare Tokio v1.18.3 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5051">#5051</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/05e661490b87a3d60a8342535bdc9d213048519c"><code>05e6614</code></a> chore: don't use <code>once_cell</code> for 1.18.x LTS release (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/5048">#5048</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/c0746b6a300f558410e719e27d2d4855f5407262"><code>c0746b6</code></a> chore: prepare Tokio v1.20.1 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4861">#4861</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.19.2...tokio-1.20.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.19.2&new-version=1.20.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 21:49:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2246" class=".btn">#2246</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in corda-4-8-all-in-one Fixes #2064
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: charelle <charelle.wrk@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 08:49:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2245" class=".btn">#2245</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump json5 from 2.2.0 to 2.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json5](https://github.com/json5/json5) from 2.2.0 to 2.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/releases">json5's releases</a>.</em></p>
<blockquote>
<h2>v2.2.2</h2>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h2>v2.2.1</h2>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/json5/json5/blob/main/CHANGELOG.md">json5's changelog</a>.</em></p>
<blockquote>
<h3>v2.2.2 [<a href="https://github.com/json5/json5/tree/v2.2.2">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.1...v2.2.2">diff</a>]</h3>
<ul>
<li>Fix: Properties with the name <code>__proto__</code> are added to objects and arrays.
(<a href="https://github-redirect.dependabot.com/json5/json5/issues/199">#199</a>) This also fixes a prototype pollution vulnerability reported by
Jonathan Gregson! (<a href="https://github-redirect.dependabot.com/json5/json5/issues/295">#295</a>).</li>
</ul>
<h3>v2.2.1 [<a href="https://github.com/json5/json5/tree/v2.2.1">code</a>, <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.1">diff</a>]</h3>
<ul>
<li>Fix: Removed dependence on minimist to patch CVE-2021-44906. (<a href="https://github-redirect.dependabot.com/json5/json5/issues/266">#266</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/json5/json5/commit/14f8cb186e8abdfaccf6527171da7b1224374650"><code>14f8cb1</code></a> 2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/10cc7ca9169b59c5e0f5afc03dbd870cd06bcc46"><code>10cc7ca</code></a> docs: update CHANGELOG for v2.2.2</li>
<li><a href="https://github.com/json5/json5/commit/7774c1097993bc3ce9f0ac4b722a32bf7d6871c8"><code>7774c10</code></a> fix: add <strong>proto</strong> to objects and arrays</li>
<li><a href="https://github.com/json5/json5/commit/edde30abd8b22facf2c06c72586b9f6edf12700d"><code>edde30a</code></a> Readme: slight tweak to intro</li>
<li><a href="https://github.com/json5/json5/commit/97286f8bd542c89dcee096bc05dd28ed2dfc1e16"><code>97286f8</code></a> Improve example in readme</li>
<li><a href="https://github.com/json5/json5/commit/d720b4fe4ad800b726da6b0f43c8454c4310fe8d"><code>d720b4f</code></a> Improve readme (e.g. explain JSON5 better!) (<a href="https://github-redirect.dependabot.com/json5/json5/issues/291">#291</a>)</li>
<li><a href="https://github.com/json5/json5/commit/910ce25914ed366a39a610b17bcd581b5da02d32"><code>910ce25</code></a> docs: fix spelling of Aseem</li>
<li><a href="https://github.com/json5/json5/commit/2aab4dd2a7c212dd4af7b91f29aa315c20251b92"><code>2aab4dd</code></a> test: require tap as t in cli tests</li>
<li><a href="https://github.com/json5/json5/commit/6d426865cec0ba7e20d4a98341e61cf26176b8fb"><code>6d42686</code></a> test: remove mocha syntax from tests</li>
<li><a href="https://github.com/json5/json5/commit/4798b9dbde850c8e84e59ac58ba2894ef184434d"><code>4798b9d</code></a> docs: update installation and usage for modules</li>
<li>Additional commits viewable in <a href="https://github.com/json5/json5/compare/v2.2.0...v2.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=json5&package-manager=npm_and_yarn&previous-version=2.2.0&new-version=2.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cactus/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-02 04:53:29 +0000 UTC
    </div>
</div>

