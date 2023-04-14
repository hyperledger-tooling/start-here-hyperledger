---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    build(deps): Bump h2 from 0.3.16 to 0.3.17 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.16 to 0.3.17.
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
<li>See full diff in <a href="https://github.com/hyperium/h2/compare/v0.3.16...v0.3.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.16&new-version=0.3.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 17:09:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    build(deps): Bump h2 from 0.3.16 to 0.3.17 in /common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [h2](https://github.com/hyperium/h2) from 0.3.16 to 0.3.17.
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
<li>See full diff in <a href="https://github.com/hyperium/h2/compare/v0.3.16...v0.3.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=h2&package-manager=cargo&previous-version=0.3.16&new-version=0.3.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 17:09:10 +0000 UTC
    </div>
</div>

