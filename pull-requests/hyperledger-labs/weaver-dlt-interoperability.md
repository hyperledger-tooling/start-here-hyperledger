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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Bump miow from 0.2.1 to 0.2.2 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [miow](https://github.com/yoshuawuyts/miow) from 0.2.1 to 0.2.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/yoshuawuyts/miow/commit/6fd7b9cfb5f5998dc6772803354b05815e579bb8"><code>6fd7b9c</code></a> Bump version to 0.2.2</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/550efc2e9608b72e971d659a01f2d02a3a27e1bc"><code>550efc2</code></a> Merge branch 'fix-sockaddr-convertion-v0.2.x' into 0.2.x</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/ca8db5365495d6da42b2f26f2062fb5e12b6c329"><code>ca8db53</code></a> Stop using from_ne_bytes to be compatible with Rust &lt; 1.32.0</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/3e217e34994923c4ef99aa3209aa9448b9e8b798"><code>3e217e3</code></a> Bump net2 dep to 0.2.36 without invalid SocketAddr convertion</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/27b77cc870b922d305015841978b581ceb18e3b9"><code>27b77cc</code></a> Adapt to winapi 0.2</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/2783715269d56a0020160179c0f2ba883d12d874"><code>2783715</code></a> Safely convert SocketAddr into raw SOCKADDR</li>
<li><a href="https://github.com/yoshuawuyts/miow/commit/f6662ef11d1aac309aea5a6548c1a2d35c1de6e9"><code>f6662ef</code></a> Clarify wording of license information in README.</li>
<li>See full diff in <a href="https://github.com/yoshuawuyts/miow/compare/0.2.1...0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=miow&package-manager=cargo&previous-version=0.2.1&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 21:12:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    Bump tokio from 0.2.21 to 1.8.4 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 0.2.21 to 1.8.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tokio-rs/tokio/releases">tokio's releases</a>.</em></p>
<blockquote>
<h2>Tokio v1.8.4</h2>
<h1>1.8.4 (November 15, 2021)</h1>
<p>This release backports a bugfix for a data race when sending and receiving on a
closed <code>oneshot</code> channel ([RUSTSEC-2021-0124]) from v1.13.1.</p>
<h3>Fixed</h3>
<ul>
<li>sync: fix a data race between <code>oneshot::Sender::send</code> and awaiting a
<code>oneshot::Receiver</code> when the oneshot has been closed (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4226">#4226</a>)</li>
</ul>
<h2>Tokio v1.8.3</h2>
<h1>1.8.3 (July 22, 2021)</h1>
<p>This release backports two fixes from 1.9.0</p>
<h3>Fixed</h3>
<ul>
<li>Fix leak if output of future panics on drop (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3967">#3967</a>)</li>
<li>Fix leak in <code>LocalSet</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3978">#3978</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3967">#3967</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3967">tokio-rs/tokio#3967</a>
<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3978">#3978</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3978">tokio-rs/tokio#3978</a></p>
<h2>Tokio 1.8.2</h2>
<p>Fixes a missed edge case from 1.8.1.</p>
<h3>Fixed</h3>
<ul>
<li>runtime: drop canceled future on next poll (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3965">#3965</a>)</li>
</ul>
<h2>Tokio 1.8.1</h2>
<p>Forward ports 1.5.1 fixes.</p>
<h3>Fixed</h3>
<ul>
<li>runtime: remotely abort tasks on <code>JoinHandle::abort</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3934">#3934</a>)</li>
</ul>
<p><a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3934">#3934</a>: <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/pull/3934">tokio-rs/tokio#3934</a></p>
<h2>tokio-1.8.0</h2>
<h1>1.8.0 (July 2, 2021)</h1>
<h3>Added</h3>
<ul>
<li>io: add <code>get_{ref,mut}</code> methods to <code>AsyncFdReadyGuard</code> and <code>AsyncFdReadyMutGuard</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3807">#3807</a>)</li>
<li>io: efficient implementation of vectored writes for <code>BufWriter</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3163">#3163</a>)</li>
<li>net: add ready/try methods to <code>NamedPipe{Client,Server}</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3866">#3866</a>, <a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3899">#3899</a>)</li>
<li>sync: add <code>watch::Receiver::borrow_and_update</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3813">#3813</a>)</li>
<li>sync: implement <code>From&lt;T&gt;</code> for <code>OnceCell&lt;T&gt;</code> (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3877">#3877</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/2273eb1a1a9c9cfa2bd998c2215239e6fe1ed57a"><code>2273eb1</code></a> chore: fix CI on master (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4008">#4008</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/249f05c0bb6694bb111b4604541e38db840cd28c"><code>249f05c</code></a> chore: fix output of macro after new rustc release (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4189">#4189</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/2bf613206a29da5a5d262e0b44bb7fac1d40fa31"><code>2bf6132</code></a> macros: fix type resolution error in #[tokio::main] (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4176">#4176</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/c9228bf7513da8b2553788195190bfa25d546ef8"><code>c9228bf</code></a> macros: make tokio-macros attributes more IDE friendly (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4162">#4162</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/441427c99356192023cf896b6f8bb747af29223c"><code>441427c</code></a> macros: fix wrong error messages (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4067">#4067</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/cc7d9e1bbf0bb71bf90759d007ca143196a81823"><code>cc7d9e1</code></a> chore: explicitly relaxed clippy lint for runtime entry macro (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4030">#4030</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/f49b7fc6da7a6e76b40a12ffebddcd6de9987196"><code>f49b7fc</code></a> tokio-macros: compat with clippy::unwrap_used (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3926">#3926</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/ea87e4ec44c5c0530d5e6c29e7d09ba818e07b5b"><code>ea87e4e</code></a> net: fix the uds_datagram tests with the latest nightly stdlib (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3952">#3952</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/e2e7b5e0ade0aa499fdb9a808b07833643457f7b"><code>e2e7b5e</code></a> examples: replace time crate with httpdate (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/4169">#4169</a>)</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9a58f7fbe76c72fdd70107223410bcf8106c3635"><code>9a58f7f</code></a> tests: update Nix to 0.22.0 (<a href="https://github-redirect.dependabot.com/tokio-rs/tokio/issues/3951">#3951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/tokio-rs/tokio/compare/tokio-0.2.21...tokio-1.8.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=0.2.21&new-version=1.8.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 21:47:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Bump hyper from 0.13.5 to 0.13.10 in /core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [hyper](https://github.com/hyperium/hyper) from 0.13.5 to 0.13.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/releases">hyper's releases</a>.</em></p>
<blockquote>
<h2>v0.13.10</h2>
<h2>Bug Fixes</h2>
<ul>
<li>
<p><strong>http1:</strong> fix server misinterpretting multiple Transfer-Encoding headers (<a href="https://github.com/hyperium/hyper/commit/6d9e5f9fd1691a0befe70b5b5be3393e45cac66a">6d9e5f9f</a>)</p>
<p>See <a href="https://github.com/hyperium/hyper/security/advisories/GHSA-6hfq-h8hq-87mf">https://github.com/hyperium/hyper/security/advisories/GHSA-6hfq-h8hq-87mf</a></p>
</li>
</ul>
<h2>v0.13.9</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong> fix panic when addrs in ConnectingTcpRemote is empty (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2292">#2292</a>) (<a href="https://github.com/hyperium/hyper/commit/01103da5d9b15e2a7fdc2f1dfec2c23a890d5c16">01103da5</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2291">#2291</a>)</li>
<li><strong>http2:</strong> reschedule keep alive interval timer once a pong is received (<a href="https://github.com/hyperium/hyper/commit/2a938d96aec62603dcb548834676ae2c71ae8be2">2a938d96</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2310">#2310</a>)</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>client:</strong>
<ul>
<li>add <code>HttpConnector::set_local_addresses</code> to set both IPv6 and IPv4 local addrs ( (<a href="https://github.com/hyperium/hyper/commit/fb19f3a86997af1c8a31a7d5ce6f2b018c9b5a0d">fb19f3a8</a>)</li>
<li>Add accessors to <code>Connected</code> fields (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2290">#2290</a>) (<a href="https://github.com/hyperium/hyper/commit/2dc9768d2d3884afa20c08b7cd8782c870d925d2">2dc9768d</a>)</li>
</ul>
</li>
</ul>
<h2>v0.13.8</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>http1:</strong> return error if user body ends prematurely (<a href="https://github.com/hyperium/hyper/commit/1ecbcbb119e221f60d37b934b81d18493ebded1b">1ecbcbb1</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2263">#2263</a>)</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>lib:</strong> Setting <code>http1_writev(true)</code> will now force writev queue usage (<a href="https://github.com/hyperium/hyper/commit/187c22afb5a13d4fa9a3b938a1d71b11b337ac97">187c22af</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2282">#2282</a>)</li>
<li><strong>server:</strong> implement <code>AsRawFd</code> for <code>AddrStream</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2246">#2246</a>) (<a href="https://github.com/hyperium/hyper/commit/b5d5e21449eb613a3c92dcced6f38d227e405594">b5d5e214</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2245">#2245</a>)</li>
</ul>
<h2>v0.13.7</h2>
<h2>Bug Fixes</h2>
<ul>
<li><strong>client:</strong> don't panic in DNS resolution when task cancelled (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2229">#2229</a>) (<a href="https://github.com/hyperium/hyper/commit/0d0d3635476ba22e5a2b39b0e4b243f57f1f36d2">0d0d3635</a>)</li>
</ul>
<h2>Features</h2>
<ul>
<li><strong>client:</strong> impl tower_service::Service for &amp;Client (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2089">#2089</a>) (<a href="https://github.com/hyperium/hyper/commit/77c3b5bc0c0d58ecd9f3c004287f65b8a94cc429">77c3b5bc</a>)</li>
<li><strong>http2:</strong> configure HTTP/2 frame size in the high-level builders too (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2214">#2214</a>) (<a href="https://github.com/hyperium/hyper/commit/2354a7eec352b1f72cd8989d29d73dff211403a1">2354a7ee</a>)</li>
<li><strong>lib:</strong> Move from <code>log</code> to <code>tracing</code> in a backwards-compatible way (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2204">#2204</a>) (<a href="https://github.com/hyperium/hyper/commit/9832aef9eeaeff8979354d5de04b8706ff79a233">9832aef9</a>)</li>
</ul>
<h2>v0.13.6</h2>
<h2>Features</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/hyperium/hyper/blob/v0.13.10/CHANGELOG.md">hyper's changelog</a>.</em></p>
<blockquote>
<h3>v0.13.10 (2021-02-05)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>http1:</strong> fix server misinterpretting multiple Transfer-Encoding headers (<a href="https://github.com/hyperium/hyper/commit/6d9e5f9fd1691a0befe70b5b5be3393e45cac66a">6d9e5f9f</a>)</li>
</ul>
<h3>v0.13.9 (2020-11-02)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> fix panic when addrs in ConnectingTcpRemote is empty (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2292">#2292</a>) (<a href="https://github.com/hyperium/hyper/commit/01103da5d9b15e2a7fdc2f1dfec2c23a890d5c16">01103da5</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2291">#2291</a>)</li>
<li><strong>http2:</strong> reschedule keep alive interval timer once a pong is received (<a href="https://github.com/hyperium/hyper/commit/2a938d96aec62603dcb548834676ae2c71ae8be2">2a938d96</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2310">#2310</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>client:</strong>
<ul>
<li>add <code>HttpConnector::set_local_addresses</code> to set both IPv6 and IPv4 local addrs ( (<a href="https://github.com/hyperium/hyper/commit/fb19f3a86997af1c8a31a7d5ce6f2b018c9b5a0d">fb19f3a8</a>)</li>
<li>Add accessors to <code>Connected</code> fields (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2290">#2290</a>) (<a href="https://github.com/hyperium/hyper/commit/2dc9768d2d3884afa20c08b7cd8782c870d925d2">2dc9768d</a>)</li>
</ul>
</li>
</ul>
<h3>v0.13.8 (2020-09-18)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>http1:</strong> return error if user body ends prematurely (<a href="https://github.com/hyperium/hyper/commit/1ecbcbb119e221f60d37b934b81d18493ebded1b">1ecbcbb1</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2263">#2263</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>lib:</strong> Setting <code>http1_writev(true)</code> will now force writev queue usage (<a href="https://github.com/hyperium/hyper/commit/187c22afb5a13d4fa9a3b938a1d71b11b337ac97">187c22af</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2282">#2282</a>)</li>
<li><strong>server:</strong> implement <code>AsRawFd</code> for <code>AddrStream</code> (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2246">#2246</a>) (<a href="https://github.com/hyperium/hyper/commit/b5d5e21449eb613a3c92dcced6f38d227e405594">b5d5e214</a>, closes <a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2245">#2245</a>)</li>
</ul>
<h3>v0.13.7 (2020-07-13)</h3>
<h4>Bug Fixes</h4>
<ul>
<li><strong>client:</strong> don't panic in DNS resolution when task cancelled (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2229">#2229</a>) (<a href="https://github.com/hyperium/hyper/commit/0d0d3635476ba22e5a2b39b0e4b243f57f1f36d2">0d0d3635</a>)</li>
</ul>
<h4>Features</h4>
<ul>
<li><strong>client:</strong> impl tower_service::Service for &amp;Client (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2089">#2089</a>) (<a href="https://github.com/hyperium/hyper/commit/77c3b5bc0c0d58ecd9f3c004287f65b8a94cc429">77c3b5bc</a>)</li>
<li><strong>http2:</strong> configure HTTP/2 frame size in the high-level builders too (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2214">#2214</a>) (<a href="https://github.com/hyperium/hyper/commit/2354a7eec352b1f72cd8989d29d73dff211403a1">2354a7ee</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper/commit/17f54264ac28b84208ccbc4119aba0573d2f7c1f"><code>17f5426</code></a> v0.13.10</li>
<li><a href="https://github.com/hyperium/hyper/commit/6d9e5f9fd1691a0befe70b5b5be3393e45cac66a"><code>6d9e5f9</code></a> fix(http1): fix server misinterpretting multiple Transfer-Encoding headers</li>
<li><a href="https://github.com/hyperium/hyper/commit/42560c7c40d8f934658624114fda4eb819cefda8"><code>42560c7</code></a> v0.13.9</li>
<li><a href="https://github.com/hyperium/hyper/commit/2a938d96aec62603dcb548834676ae2c71ae8be2"><code>2a938d9</code></a> fix(server): reschedule keep alive interval timer once a pong is received</li>
<li><a href="https://github.com/hyperium/hyper/commit/f2886417925da2c62637b8509cd40ded0b848333"><code>f288641</code></a> test(server): test server keep alive by counting number of pings</li>
<li><a href="https://github.com/hyperium/hyper/commit/fb19f3a86997af1c8a31a7d5ce6f2b018c9b5a0d"><code>fb19f3a</code></a> feat(client): add <code>HttpConnector::set_local_addresses</code> to set both IPv6 and I...</li>
<li><a href="https://github.com/hyperium/hyper/commit/02732bef0c1accb441b9b14c07cb2c494234a682"><code>02732be</code></a> chore(dependencies): update pin-project to 1.0 (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2298">#2298</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/2dc9768d2d3884afa20c08b7cd8782c870d925d2"><code>2dc9768</code></a> feat(client): Add accessors to <code>Connected</code> fields (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2290">#2290</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/01103da5d9b15e2a7fdc2f1dfec2c23a890d5c16"><code>01103da</code></a> fix(client): fix panic when addrs in ConnectingTcpRemote is empty (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2292">#2292</a>)</li>
<li><a href="https://github.com/hyperium/hyper/commit/523d66a41ffe0429530241c381070fb490618a4a"><code>523d66a</code></a> refactor(body): fix unused sync_wrapper when stream feature disabled (<a href="https://github-redirect.dependabot.com/hyperium/hyper/issues/2287">#2287</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/hyperium/hyper/compare/v0.13.5...v0.13.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=hyper&package-manager=cargo&previous-version=0.13.5&new-version=0.13.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/weaver-dlt-interoperability/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 20:29:15 +0000 UTC
    </div>
</div>

