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
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    build(deps): bump hyper from 0.14.11 to 0.14.15 in /rust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [hyper](https://github.com/hyperium/hyper) from 0.14.11 to 0.14.15.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/releases">hyper's releases</a>.</em></p>
<blockquote>
<h2>v0.14.15</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong> cancel blocking DNS lookup if <code>GaiFuture</code> is dropped (<a href="https://github.com/hyperium/hyper/commit/174b553d">174b553d</a>)</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>http1:</strong> add <code>http1_writev(bool)</code> options to Client and Server builders, to allow forcing vectored writes (<a href="https://github.com/hyperium/hyper/commit/80627141">80627141</a>)</li>
<li><strong>upgrade:</strong> allow http upgrades with any body type (<a href="https://github.com/hyperium/hyper/commit/ab469eb3c6cd5e7a035d734f3d21ff4d2d6a21ab">ab469eb3</a>)</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/luqmana"><code>@​luqmana</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/hyperium/hyper/pull/2680">hyperium/hyper#2680</a></li>
<li><a href="https://github.com/whentze"><code>@​whentze</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/hyperium/hyper/pull/2688">hyperium/hyper#2688</a></li>
<li><a href="https://github.com/ahmedsobeh"><code>@​ahmedsobeh</code></a> made their first contribution in <a href="https://github-redirect.dependabot.com/hyperium/hyper/pull/2689">hyperium/hyper#2689</a></li>
</ul>
<h2>v0.14.14</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong>
<ul>
<li>make ResponseFuture implement Sync (<a href="https://github.com/hyperium/hyper/commit/bd6c35b98f9513f14ed9cecad933bc7fdb8635ea">bd6c35b9</a>)</li>
<li>remove ipv6 square brackets before resolving (<a href="https://github.com/hyperium/hyper/commit/910e02687df3245aae4bc519fb0bd7eb6a34db7d">910e0268</a>)</li>
</ul>
</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>http2:</strong> always include original h2 error on broken pipe (<a href="https://github.com/hyperium/hyper/commit/6169db250c932dd012d391389826cd34833077b4">6169db25</a>)</li>
<li><strong>server:</strong> Remove Send + Sync requirement for Body in with_graceful_shutdown (<a href="https://github.com/hyperium/hyper/commit/1d553e52c6953ea3b039f5c3f89d35cb56e2436a">1d553e52</a>)</li>
</ul>
<h2>v0.14.13</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong> don't reuse a connection while still flushing (<a href="https://github.com/hyperium/hyper/commit/c88011da4ed5b5ca9107c4a2339a7ab054c5f27f">c88011da</a>)</li>
<li><strong>server:</strong> convert panic to error if Connection::without_shutdown called on HTTP/2 conn (<a href="https://github.com/hyperium/hyper/commit/ea3e228287e714b97aa44c840a487abd3a915e15">ea3e2282</a>)</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>ffi:</strong> add hyper_request_set_uri_parts (<a href="https://github.com/hyperium/hyper/commit/a54689b921ca16dd0f29b3f4a74feae60218db34">a54689b9</a>)</li>
<li><strong>lib:</strong>
<ul>
<li>Export more things with Cargo features (server, !http1, !http2) (<a href="https://github.com/hyperium/hyper/commit/0a4b56acb82ef41a3336f482b240c67c784c434f">0a4b56ac</a>)</li>
<li>Export rt module independently of Cargo features (<a href="https://github.com/hyperium/hyper/commit/cf6f62c71eda3b3a8732d86387e4ed8711cf9a86">cf6f62c7</a>)</li>
</ul>
</li>
</ul>
<h2>v0.14.12</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>ffi:</strong> on_informational callback had no headers (<a href="https://github.com/hyperium/hyper/commit/39b6d01aa0e520077bb25e16811f5ece00a224d6">39b6d01a</a>)</li>
<li><strong>http1:</strong> apply header title case for consecutive dashes (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2613">#2613</a>) (<a href="https://github.com/hyperium/hyper/commit/684f2fa76d44fa2b1b063ad0443a1b0d16dfad0e">684f2fa7</a>)</li>
<li><strong>http2:</strong> improve errors emitted by HTTP2 <code>Upgraded</code> stream shutdown (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2622">#2622</a>) (<a href="https://github.com/hyperium/hyper/commit/be08648e8298cdb13e9879ee761a73f827268962">be08648e</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/blob/master/CHANGELOG.md">hyper's changelog</a>.</em></p>
<blockquote>
<h3>v0.14.15 (2021-11-16)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> cancel blocking DNS lookup if <code>GaiFuture</code> is dropped (<a href="https://github.com/hyperium/hyper/commit/174b553d">174b553d</a></li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>http1:</strong> add <code>http1_writev(bool)</code> options to Client and Server builders, to allow forcing vectored writes (<a href="https://github.com/hyperium/hyper/commit/80627141">80627141</a>)</li>
<li><strong>upgrade:</strong> allow http upgrades with any body type (<a href="https://github.com/hyperium/hyper/commit/ab469eb3c6cd5e7a035d734f3d21ff4d2d6a21ab">ab469eb3</a>)</li>
</ul>
<h3>v0.14.14 (2021-10-22)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong>
<ul>
<li>make ResponseFuture implement Sync (<a href="https://github.com/hyperium/hyper/commit/bd6c35b98f9513f14ed9cecad933bc7fdb8635ea">bd6c35b9</a>)</li>
<li>remove ipv6 square brackets before resolving (<a href="https://github.com/hyperium/hyper/commit/910e02687df3245aae4bc519fb0bd7eb6a34db7d">910e0268</a>)</li>
</ul>
</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>h2:</strong> always include original h2 error on broken pipe (<a href="https://github.com/hyperium/hyper/commit/6169db250c932dd012d391389826cd34833077b4">6169db25</a>)</li>
<li><strong>server:</strong> Remove Send + Sync requirement for Body in with_graceful_shutdown (<a href="https://github.com/hyperium/hyper/commit/1d553e52c6953ea3b039f5c3f89d35cb56e2436a">1d553e52</a>)</li>
</ul>
<h3>v0.14.13 (2021-09-16)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> don't reuse a connection while still flushing (<a href="https://github.com/hyperium/hyper/commit/c88011da4ed5b5ca9107c4a2339a7ab054c5f27f">c88011da</a>)</li>
<li><strong>server:</strong> convert panic to error if Connection::without_shutdown called on HTTP/2 conn (<a href="https://github.com/hyperium/hyper/commit/ea3e228287e714b97aa44c840a487abd3a915e15">ea3e2282</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>ffi:</strong> add hyper_request_set_uri_parts (<a href="https://github.com/hyperium/hyper/commit/a54689b921ca16dd0f29b3f4a74feae60218db34">a54689b9</a>)</li>
<li><strong>lib:</strong>
<ul>
<li>Export more things with Cargo features (server, !http1, !http2) (<a href="https://github.com/hyperium/hyper/commit/0a4b56acb82ef41a3336f482b240c67c784c434f">0a4b56ac</a>)</li>
<li>Export rt module independently of Cargo features (<a href="https://github.com/hyperium/hyper/commit/cf6f62c71eda3b3a8732d86387e4ed8711cf9a86">cf6f62c7</a>)</li>
</ul>
</li>
</ul>
<h3>v0.14.12 (2021-08-24)</h3>
<h4>Bug Fixes</h4>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper/commit/d0b1d9ed3a10013ab356bc7d9b283e179857a672"><code>d0b1d9e</code></a> v0.14.15</li>
<li><a href="https://github.com/hyperium/hyper/commit/a1502e1067d28b5fc1883e48ac7daacf2fbe4b9e"><code>a1502e1</code></a> docs(http1): clarify HTTP1 preserve case option</li>
<li><a href="https://github.com/hyperium/hyper/commit/a12db28542e2ecd6f67459b4777a24cb71b9bdc8"><code>a12db28</code></a> docs(upgrade): add module documentation for HTTP upgrades</li>
<li><a href="https://github.com/hyperium/hyper/commit/7f5e853dd86b641aa9927f02105bf130d8aaaca3"><code>7f5e853</code></a> refactor(benches): make benchmark names more consistent</li>
<li><a href="https://github.com/hyperium/hyper/commit/174b553d2d877a332090b0df43375e7edb685671"><code>174b553</code></a> fit(client): cancel blocking DNS lookup if GaiFuture dropped (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2689">#2689</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/913be88f7155ea4695c7f8098d968bf1f340f8be"><code>913be88</code></a> docs(client): fix missing feature attrs in another doctest</li>
<li><a href="https://github.com/hyperium/hyper/commit/3221f573d2dc6162dcf12f02ee68e4c4cbaf149d"><code>3221f57</code></a> docs(body) fix doctest failing due to missing features</li>
<li><a href="https://github.com/hyperium/hyper/commit/80627141ede3cdaf37b833ee91d08be0af0f5c84"><code>8062714</code></a> feat(http1): Add <code>http1_writev(bool)</code> to client and server Builders</li>
<li><a href="https://github.com/hyperium/hyper/commit/ab469eb3c6cd5e7a035d734f3d21ff4d2d6a21ab"><code>ab469eb</code></a> feat(upgrade): allow http upgrades with any body type</li>
<li><a href="https://github.com/hyperium/hyper/commit/b5022f3854d1f9ed3e76233dd63f319efc3b8f47"><code>b5022f3</code></a> v0.14.14</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/hyper/compare/v0.14.11...v0.14.15">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyper&package-manager=cargo&previous-version=0.14.11&new-version=0.14.15)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-17 01:36:29 +0000 UTC
    </div>
</div>

