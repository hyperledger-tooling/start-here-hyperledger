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
                PR <a href="https://github.com/hyperledger/cactus/pull/2087" class=".btn">#2087</a>
            </td>
            <td>
                <b>
                    fix: Lint Warnings resolved for batch 7/26 #1356 : Commit to be reviewed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: batch 7/26 of lint warning fixes #1356(fixed 5 warnings, partial solution): 

Changes made:
- Fixed lint warnings associated with any-type for truthyness and nonBlankString checking
- Fixed lint warnings associated with Unexpected any, edited type-aliases in logger
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 09:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2086" class=".btn">#2086</a>
            </td>
            <td>
                <b>
                    refactor(cmd-api-server): clean up configuration parameters gitguardi…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …an scanner test

test

Signed-off-by: ruzell22 <ruzell.vince.aquino@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 06:31:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2085" class=".btn">#2085</a>
            </td>
            <td>
                <b>
                    build(deps): bump thread_local from 1.1.0 to 1.1.4 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [thread_local](https://github.com/Amanieu/thread_local-rs) from 1.1.0 to 1.1.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/4a54e5702e0968bdda77366738ba646f646044e8"><code>4a54e57</code></a> Bump version to 1.1.4</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/ebf8b45fa2b427ede21b75d263a8c99150526dd1"><code>ebf8b45</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/34">#34</a> from ibraheemdev/patch-1</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/3d69afaab242fc1dd3a0658eb363b2df5e02fcd6"><code>3d69afa</code></a> Fix memory ordering in <code>RawIter::next</code></li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/c7d8dcdf4b93a5d80ec4075c3d8e7351c1a32012"><code>c7d8dcd</code></a> Bump version to 1.1.3</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/5e8bbf2b4f17d9c056d17de324d5a8465d20f96e"><code>5e8bbf2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/30">#30</a> from Marwes/fix_drop</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/a44b836f90e0317d256ed1dd4cff745feff285ea"><code>a44b836</code></a> fix: Drop the value in the ThreadLocal on drop</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/322cf34816a62f1519d005cc44d623741740324e"><code>322cf34</code></a> Bump version to 1.1.2</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/dca4007eafb16fe189caea4fe08a6b80223b3fb1"><code>dca4007</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/Amanieu/thread_local-rs/issues/29">#29</a> from Kestrer/raw-iter</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/33ad4052309ba8b48b7436bf82d66be07103fa3f"><code>33ad405</code></a> Add #[inline] to non-generic functions</li>
<li><a href="https://github.com/Amanieu/thread_local-rs/commit/810c043ff71ef66b96ca5d92319df4aa7134bf44"><code>810c043</code></a> Implement iterator logic in RawIter</li>
<li>Additional commits viewable in <a href="https://github.com/Amanieu/thread_local-rs/compare/v1.1.0...1.1.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=thread_local&package-manager=cargo&previous-version=1.1.0&new-version=1.1.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-17 01:40:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2084" class=".btn">#2084</a>
            </td>
            <td>
                <b>
                    build(deps): bump hyper from 0.13.9 to 0.14.8 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [hyper](https://github.com/hyperium/hyper) from 0.13.9 to 0.14.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/releases">hyper's releases</a>.</em></p>
<blockquote>
<h2>v0.14.8</h2>
<h2>Features</h2>
<ul>
<li><strong>client:</strong> allow to config http2 max concurrent reset streams (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2535">#2535</a>) (<a href="https://github.com/hyperium/hyper/commit/b9916c410182c6225e857f0cded355ea1b74c865">b9916c41</a>)</li>
<li><strong>error:</strong> add <code>Error::is_parse_too_large</code> and <code>Error::is_parse_status</code> methods (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2538">#2538</a>) (<a href="https://github.com/hyperium/hyper/commit/960a69a5878ede82c56f50ac1444a9e75e885a8f">960a69a5</a>)</li>
<li><strong>http2:</strong>
<ul>
<li>Implement Client-side CONNECT support over HTTP/2 (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2523">#2523</a>) (<a href="https://github.com/hyperium/hyper/commit/5442b6faddaff9aeb7c073031a3b7aa4497fda4d">5442b6fa</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2508">#2508</a>)</li>
<li>allow HTTP/2 requests by ALPN when http2_only is unset (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2527">#2527</a>) (<a href="https://github.com/hyperium/hyper/commit/be9677a1e782d33c4402772e0fc4ef0a4c49d507">be9677a1</a>)</li>
</ul>
</li>
</ul>
<h2>Performance</h2>
<ul>
<li><strong>http2:</strong> reduce amount of adaptive window pings as BDP stabilizes (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2550">#2550</a>) (<a href="https://github.com/hyperium/hyper/commit/4cd06bf2">4cd06bf2</a>)</li>
</ul>
<h2>v0.14.6</h2>
<h2>Features</h2>
<ul>
<li><strong>client:</strong> add option to allow misplaced spaces in HTTP/1 responses (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2506">#2506</a>) (<a href="https://github.com/hyperium/hyper/commit/11345394d968d4817e1a0ee2550228ac0ae7ce74">11345394</a>)</li>
<li><strong>http1:</strong> add options to preserve header casing (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2480">#2480</a>) (<a href="https://github.com/hyperium/hyper/commit/dbea7716f157896bf7d2d417be7b4e382e7dc34f">dbea7716</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2313">#2313</a>)</li>
</ul>
<h2>v0.14.5</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong> omit default port from automatic Host headers (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2441">#2441</a>) (<a href="https://github.com/hyperium/hyper/commit/0b11eee9bde421cdc1680cadabfd38c5aff8e62f">0b11eee9</a>)</li>
<li><strong>headers:</strong> Support multiple Content-Length values on same line (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2471">#2471</a>) (<a href="https://github.com/hyperium/hyper/commit/48fdaf160689f333e9bb63388d0b1d0fa29a1391">48fdaf16</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2470">#2470</a>)</li>
<li><strong>server:</strong> skip automatic Content-Length headers when not allowed (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2216">#2216</a>) (<a href="https://github.com/hyperium/hyper/commit/8cbf9527dfb313b3f84fcd83260c5c72ce4a1beb">8cbf9527</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2215">#2215</a>)</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>client:</strong> allow HTTP/0.9 responses behind a flag (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2473">#2473</a>) (<a href="https://github.com/hyperium/hyper/commit/68d4e4a3db91fb43f41a8c4fce1175ddb56816af">68d4e4a3</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2468">#2468</a>)</li>
<li><strong>server:</strong> add <code>AddrIncoming::from_listener</code> constructor (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2439">#2439</a>) (<a href="https://github.com/hyperium/hyper/commit/4c946af49cc7fbbc6bd4894283a654625c2ea383">4c946af4</a>)</li>
</ul>
<h2>v0.14.4</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>build</strong>: Fix compile error when only <code>http1</code> feature was enabled.</li>
</ul>
<h2>v0.14.3</h2>
<h2>Bug Fixes</h2>
<ul>
<li>
<p><strong>client:</strong> HTTP/1 client &quot;Transfer-Encoding&quot; repair code would panic (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2410">#2410</a>) (<a href="https://github.com/hyperium/hyper/commit/2c8121f1735aa8efeb0d5e4ef595363c373ba470">2c8121f1</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2409">#2409</a>)</p>
</li>
<li>
<p><strong>http1:</strong> fix server misinterpretting multiple Transfer-Encoding headers (<a href="https://github.com/hyperium/hyper/commit/8f93123efef5c1361086688fe4f34c83c89cec02">8f93123e</a>)</p>
<p>See <a href="https://github.com/hyperium/hyper/security/advisories/GHSA-6hfq-h8hq-87mf">https://github.com/hyperium/hyper/security/advisories/GHSA-6hfq-h8hq-87mf</a></p>
</li>
</ul>
<h2>Features</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/blob/master/CHANGELOG.md">hyper's changelog</a>.</em></p>
<blockquote>
<h3>v0.14.8 (2021-05-25)</h3>
<h4>Features</h4>
<ul>
<li><strong>client:</strong> allow to config http2 max concurrent reset streams (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2535">#2535</a>) (<a href="https://github.com/hyperium/hyper/commit/b9916c410182c6225e857f0cded355ea1b74c865">b9916c41</a>)</li>
<li><strong>error:</strong> add <code>Error::is_parse_too_large</code> and <code>Error::is_parse_status</code> methods (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2538">#2538</a>) (<a href="https://github.com/hyperium/hyper/commit/960a69a5878ede82c56f50ac1444a9e75e885a8f">960a69a5</a>)</li>
<li><strong>http2:</strong>
<ul>
<li>Implement Client and Server CONNECT support over HTTP/2 (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2523">#2523</a>) (<a href="https://github.com/hyperium/hyper/commit/5442b6faddaff9aeb7c073031a3b7aa4497fda4d">5442b6fa</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2508">#2508</a>)</li>
<li>allow HTTP/2 requests by ALPN when http2_only is unset (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2527">#2527</a>) (<a href="https://github.com/hyperium/hyper/commit/be9677a1e782d33c4402772e0fc4ef0a4c49d507">be9677a1</a>)</li>
</ul>
</li>
</ul>
<h4>Performance</h4>
<ul>
<li><strong>http2:</strong> reduce amount of adaptive window pings as BDP stabilizes (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2550">#2550</a>) (<a href="https://github.com/hyperium/hyper/commit/4cd06bf2">4cd06bf2</a>)</li>
</ul>
<h3>v0.14.7 (2021-04-22)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>http1:</strong> http1_title_case_headers should move Builder (<a href="https://github.com/hyperium/hyper/commit/a303b3c329e6b8ecfa1da0b9b9e94736628167e0">a303b3c3</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>server:</strong> implement forgotten settings for case preserving (<a href="https://github.com/hyperium/hyper/commit/4fd6c4cb0b58bb0831ae0f876d858aba1588d0e3">4fd6c4cb</a>)</li>
</ul>
<h3>v0.14.6 (2021-04-21)</h3>
<h4>Features</h4>
<ul>
<li><strong>client:</strong> add option to allow misplaced spaces in HTTP/1 responses (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2506">#2506</a>) (<a href="https://github.com/hyperium/hyper/commit/11345394d968d4817e1a0ee2550228ac0ae7ce74">11345394</a>)</li>
<li><strong>http1:</strong> add options to preserve header casing (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2480">#2480</a>) (<a href="https://github.com/hyperium/hyper/commit/dbea7716f157896bf7d2d417be7b4e382e7dc34f">dbea7716</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2313">#2313</a>)</li>
</ul>
<h3>v0.14.5 (2021-03-26)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> omit default port from automatic Host headers (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2441">#2441</a>) (<a href="https://github.com/hyperium/hyper/commit/0b11eee9bde421cdc1680cadabfd38c5aff8e62f">0b11eee9</a>)</li>
<li><strong>headers:</strong> Support multiple Content-Length values on same line (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2471">#2471</a>) (<a href="https://github.com/hyperium/hyper/commit/48fdaf160689f333e9bb63388d0b1d0fa29a1391">48fdaf16</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2470">#2470</a>)</li>
<li><strong>server:</strong> skip automatic Content-Length headers when not allowed (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2216">#2216</a>) (<a href="https://github.com/hyperium/hyper/commit/8cbf9527dfb313b3f84fcd83260c5c72ce4a1beb">8cbf9527</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2215">#2215</a>)</li>
</ul>
<h4>Features</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper/commit/e61b494e3b6c7bf0247135b0c9ade516126701e9"><code>e61b494</code></a> v0.14.8</li>
<li><a href="https://github.com/hyperium/hyper/commit/5442b6faddaff9aeb7c073031a3b7aa4497fda4d"><code>5442b6f</code></a> feat(http2): Implement Client-side CONNECT support over HTTP/2 (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2523">#2523</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/be9677a1e782d33c4402772e0fc4ef0a4c49d507"><code>be9677a</code></a> feat(http2): allow HTTP/2 requests by ALPN when http2_only is unset (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2527">#2527</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/4cd06bf25661d7e43e2fdf43eabdb8508055cf3a"><code>4cd06bf</code></a> perf(http2): slow adaptive window pings as the BDP stabilizes (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2550">#2550</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/960a69a5878ede82c56f50ac1444a9e75e885a8f"><code>960a69a</code></a> feat(error): add <code>Error::is_parse_too_large</code> and <code>Error::is_parse_status</code> met...</li>
<li><a href="https://github.com/hyperium/hyper/commit/b9916c410182c6225e857f0cded355ea1b74c865"><code>b9916c4</code></a> feat(client): allow to config http2 max concurrent reset streams (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2535">#2535</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/ccba59fb1b592dfdfca4b870e0922e5ba8244825"><code>ccba59f</code></a> docs(common): remove favicon doc from sync_wrapper module (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2548">#2548</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/8a05f8eec133793899c94dcbf1520eee3b91aa50"><code>8a05f8e</code></a> docs(server): add bigger example to server module (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2539">#2539</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/e79d09396da955f235c267832312543d8230d867"><code>e79d093</code></a> docs(client): document the guarantees of cloning a <code>Client</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2540">#2540</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/d1d2f32a7358c1c7d489ebbb98f4cbfdca9bb573"><code>d1d2f32</code></a> docs(headers): no_inline doc on HeaderMap (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2525">#2525</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/hyper/compare/v0.13.9...v0.14.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyper&package-manager=cargo&previous-version=0.13.9&new-version=0.14.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-17 01:22:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2083" class=".btn">#2083</a>
            </td>
            <td>
                <b>
                    build(deps-dev): bump electron from 13.6.6 to 15.5.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [electron](https://github.com/electron/electron) from 13.6.6 to 15.5.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/electron/electron/releases">electron's releases</a>.</em></p>
<blockquote>
<h2>electron v15.5.5</h2>
<h1>Release Notes for v15.5.5</h1>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2022-1482. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34040">#34040</a></li>
<li>Backported fix for CVE-2022-1483. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34009">#34009</a></li>
<li>Backported fix for CVE-2022-1497. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34075">#34075</a></li>
</ul>
<h2>electron v15.5.4</h2>
<h1>Release Notes for v15.5.4</h1>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2022-1138. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33682">#33682</a></li>
<li>Backported fix for CVE-2022-1478. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34045">#34045</a></li>
<li>Backported fix for CVE-2022-1479. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34037">#34037</a></li>
<li>Backported fix for CVE-2022-1480. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34019">#34019</a></li>
<li>Backported fix for CVE-2022-1492. <a href="https://github-redirect.dependabot.com/electron/electron/pull/34051">#34051</a></li>
</ul>
<h2>electron v15.5.3</h2>
<h1>Release Notes for v15.5.3</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed a network service crash that could occur when using setCertificateVerifyProc. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33256">#33256</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/33255">16</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33254">17</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33253">18</a>)<!-- raw HTML omitted --></li>
<li><code>shell.openExternal()</code> now reports more detailed errors on Windows. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33656">#33656</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/33657">16</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33658">17</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33705">18</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33660">19</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<ul>
<li>Backported fix for CVE-2022-1134. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33763">#33763</a></li>
<li>Backported fix for CVE-2022-1305. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33860">#33860</a></li>
<li>Backported fix for CVE-2022-1310. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33831">#33831</a></li>
<li>Backported fix for CVE-2022-1314. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33884">#33884</a></li>
<li>Backported fix for CVE-2022-1364. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33836">#33836</a></li>
<li>Backported fix for chromium:1286816. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33679">#33679</a></li>
<li>Backported fix for chromium:1291482. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33676">#33676</a></li>
<li>Backported fix for chromium:1310761. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33856">#33856</a></li>
<li>Security: backported fix for CVE-2022-0116 and CVE-2022-1306. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33852">#33852</a></li>
<li>Security: backported fix for CVE-2022-23308. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33670">#33670</a></li>
<li>Security: backported fix for chromium:1280743. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33715">#33715</a></li>
<li>Security: backported fix for chromium:1280852. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33673">#33673</a></li>
</ul>
<h2>electron v15.5.2</h2>
<h1>Release Notes for v15.5.2</h1>
<h2>Fixes</h2>
<ul>
<li>Fixed behavior of BrowserWindow.maximize on macOS for not shown windows. <a href="https://github-redirect.dependabot.com/electron/electron/pull/33523">#33523</a> <!-- raw HTML omitted -->(Also in <a href="https://github-redirect.dependabot.com/electron/electron/pull/33535">16</a>, <a href="https://github-redirect.dependabot.com/electron/electron/pull/33537">18</a>)<!-- raw HTML omitted --></li>
</ul>
<h2>Other Changes</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/electron/electron/commit/f98885312827f3f111cfac80d71dc9a2c2d2cbc9"><code>f988853</code></a> Bump v15.5.5</li>
<li><a href="https://github.com/electron/electron/commit/8bc25e8a9de07496db6b884b228ca12d0e161f07"><code>8bc25e8</code></a> build: change upload-to-s3 vars to upload-to-storage (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34142">#34142</a>)</li>
<li><a href="https://github.com/electron/electron/commit/a8f8b507aa01c794c698f72be7cc9d0f9bb9fa5b"><code>a8f8b50</code></a> build: use azure function to hash assets instead of lambda (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34119">#34119</a>)</li>
<li><a href="https://github.com/electron/electron/commit/eb320cbbf9f887ff2ecf3c76ef8b1eff7143e49f"><code>eb320cb</code></a> build: stop uploading assets to S3 (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34112">#34112</a>)</li>
<li><a href="https://github.com/electron/electron/commit/37eab5c66e609f9d98203c58feb740d23265ea2e"><code>37eab5c</code></a> chore: cherry-pick 5be8e065f43e from chromium (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34040">#34040</a>)</li>
<li><a href="https://github.com/electron/electron/commit/fc912026e2c383c24949e4bb381eb7a07121a657"><code>fc91202</code></a> chore: cherry-pick 5361d836ae from chromium (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34009">#34009</a>)</li>
<li><a href="https://github.com/electron/electron/commit/6aa0609a9707a81611b6dceb2dbd9d779c83a040"><code>6aa0609</code></a> chore: cherry-pick 6b66a45021 from chromium (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34075">#34075</a>)</li>
<li><a href="https://github.com/electron/electron/commit/620d615fe026d654178be0a462dab3580429f55a"><code>620d615</code></a> test: fix nativeModulesEnabled in spec/webview-spec.js (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34063">#34063</a>)</li>
<li><a href="https://github.com/electron/electron/commit/ec7baba40166e9f11046cff31de180e4f652ec23"><code>ec7baba</code></a> Bump v15.5.4</li>
<li><a href="https://github.com/electron/electron/commit/f8ba4d6012c2c6a853c0b9b31e2a3816ac8b3c0c"><code>f8ba4d6</code></a> chore: cherry-pick d27d9d059b51 from angle (<a href="https://github-redirect.dependabot.com/electron/electron/issues/34045">#34045</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/electron/electron/compare/v13.6.6...v15.5.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=electron&package-manager=npm_and_yarn&previous-version=13.6.6&new-version=15.5.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-17 01:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2082" class=".btn">#2082</a>
            </td>
            <td>
                <b>
                    build(tools): software bill of materials generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a script to generate all SBoMs.
The short hand to call the script is by running
$ yarn generate-sbom
and then it saves all the different .spdx
files under ./dist/sbom/*
where the file names are derived from
the relative path of the directory of the
build definition.

Fixes #2081

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 23:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2080" class=".btn">#2080</a>
            </td>
            <td>
                <b>
                    fix(examples): fixed multiple lint errors in examples folder also changed the return types for more functions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Change

1. Fixed lint errors on utility-emissions-channel/enroll-admin-v1-endpoint.ts (line 54, col 25), insert-bamboo-harvest-endpoint.ts (line 78, col 3), insert-bookshelf-endpoint.ts (line 59, col 3), insert-shipment-endpoint.ts (line 69, col 3), list-bamboo-harvest-endpoint.ts (line 38, col 3; line 58, col 3; ), list-bookshelf-endpoint.ts (line 56, col 3), and list-shipment-endpoint.ts (line 40, col 3)
2. In order to fix changes from any to unknown, had to change the output path to directed types: (Changed OASPath return type from any object to "typeof OAS.paths["/api/v1/plugins/@hyperledger/cactus-example-carbon-accounting-backend/dao-token/get-allowance"]"
3. Removed import statements that were never used in the file (import e)
Partial Fix to #1366 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 22:34:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2079" class=".btn">#2079</a>
            </td>
            <td>
                <b>
                    fix(index.ts, emissionsRecordCOntract.ts, get-allowance-endpoint.ts): fixed lint errors on multiple files 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Change
--------------

1. Fixed lint errors on index.ts (line 578, col 25), emissionsRecordContract.ts (line 40, col 3; line 138, col 3; line 146, col 3), and endpoint.ts (line 58, col 33) 
2. In order to fix changes from any to unknown, had to change the output path to directed types: (Changed OASPath return type from any object to "typeof OAS.paths["/api/v1/plugins/@hyperledger/cactus-example-carbon-accounting-backend/dao-token/get-allowance"]"
------------------------------------------------------------
Signed-off-by: Alec Phong <alecphong@gmail.com>
Partial Fix to #1366 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 20:14:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2078" class=".btn">#2078</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha): sending transactions signed on the client-side
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add new endpoint `generate-transaction`, to create unsigned transactions
  that can be signed on the client side.
- Add a function to iroha-connector package to help signing iroha transactions
  on the client (BLP) side.
- Extend transact endpoint to accept signed transaction as an argument as well.
  New transact interface is backward compatible, all current code should work without any change.
- Add new test suite to check features implemented in this PR (i.e. signing on the client side).
- Perform minor cleanup in the connector code, remove unused fields and includes,
  fix some type related warnings.
- Perform openapi interface cleanup, format json correctly,
  mark baseConfig as required by transact (will fail otherwise),
  add error return type schemas, remove invoke-contract endpoint that was not implemented.

Closes #2077

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2076" class=".btn">#2076</a>
            </td>
            <td>
                <b>
                    fix: fixed lint errors pt2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed Lint errors throughout quourum-test-ledger.ts, also fixed a try catch error. 

Partial solution #1375 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 17:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2075" class=".btn">#2075</a>
            </td>
            <td>
                <b>
                    fix: fixed 2 lint errors that were the any type error for Typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed 2 lint errors that were the any type error for Typescript and removed Node
Partial solution to #1375 

Signed-off-by: Alec Phong <alecphong@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 19:01:32 +0000 UTC
    </div>
</div>

