---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    Bump github.com/libp2p/go-libp2p from 0.26.4 to 0.27.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/libp2p/go-libp2p](https://github.com/libp2p/go-libp2p) from 0.26.4 to 0.27.8.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/libp2p/go-libp2p/releases">github.com/libp2p/go-libp2p's releases</a>.</em></p>
<blockquote>
<h2>v0.27.8</h2>
<p>This patch release contains backports of:</p>
<ul>
<li>updating the qtls dependencies (qtls is quic-go's fork of crypto/tls). The new versions now contain a backport of the Go standard library fix included in the Go 1.20.7 / 1.19.12 release for quic-go's crypto/tls fork: <a href="https://github.com/golang/go/commit/2350afd2e8ab054390e284c95d5b089c142db017">https://github.com/golang/go/commit/2350afd2e8ab054390e284c95d5b089c142db017</a></li>
<li>core/crypto: restrict RSA keys to &lt;= 8192 bits: <a href="https://redirect.github.com/libp2p/go-libp2p/pull/2454">libp2p/go-libp2p#2454</a>. The analogous vulnerability in go-libp2p's crypto package.</li>
<li>swarm: don't open new streams over transient connections: <a href="https://redirect.github.com/libp2p/go-libp2p/pull/2450">libp2p/go-libp2p#2450</a>. This fixes a regression introduced in v0.26.0.</li>
</ul>
<p>Note that in order to be protected against the DoS attack making use of large RSA keys, it's necessary to update to this patch release AND to use the updated Go compiler (1.20.7 or 1.19.12, respectively).</p>
<p>Full Changelog: <a href="https://github.com/libp2p/go-libp2p/compare/v0.27.7...v0.27.8">https://github.com/libp2p/go-libp2p/compare/v0.27.7...v0.27.8</a></p>
<h2>v0.27.7</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: in the swarm move Connectedness emit after releasing conns <a href="https://redirect.github.com/libp2p/go-libp2p/issues/2373">#2373</a></li>
<li>identify: set stream deadlines for Identify and Identify Push streams <a href="https://redirect.github.com/libp2p/go-libp2p/issues/2382">#2382</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/libp2p/go-libp2p/compare/v0.27.6...v0.27.7">https://github.com/libp2p/go-libp2p/compare/v0.27.6...v0.27.7</a></p>
<h2>v0.27.6</h2>
<h2>What's Changed</h2>
<ul>
<li>Clean up stream scope in case of error</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/libp2p/go-libp2p/compare/v0.27.5...v0.27.6">https://github.com/libp2p/go-libp2p/compare/v0.27.5...v0.27.6</a></p>
<h2>v0.27.5</h2>
<h2>What's Changed</h2>
<ul>
<li>Dedup addresses to dial by <a href="https://github.com/MarcoPolo"><code>@​MarcoPolo</code></a> in <a href="https://redirect.github.com/libp2p/go-libp2p/pull/2322">libp2p/go-libp2p#2322</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/libp2p/go-libp2p/compare/v0.27.3...v0.27.5">https://github.com/libp2p/go-libp2p/compare/v0.27.3...v0.27.5</a></p>
<h2>v0.27.4</h2>
<h2>What's Changed</h2>
<ul>
<li>identify
<ul>
<li>Fixed an issue where we now avoid spuriously triggering pushes</li>
<li>Fixed an issue where signed peer records weren’t rejected if the signature didn’t match</li>
</ul>
</li>
<li>swarm
<ul>
<li>Fixed duplicate tracking in dial worker loop</li>
</ul>
</li>
</ul>
<h2>v0.27.3</h2>
<p>This patch release contains a fix for a rare panic that occurs on Windows systems (backport of <a href="https://redirect.github.com/libp2p/go-libp2p/pull/2276">libp2p/go-libp2p#2276</a>).</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/libp2p/go-libp2p/compare/v0.27.1...v0.27.3">https://github.com/libp2p/go-libp2p/compare/v0.27.1...v0.27.3</a></p>
<h2>v0.27.2</h2>
<h2>What's Changed</h2>
<p>quic: fix race condition when generating random holepunch packet (<a href="https://redirect.github.com/libp2p/go-libp2p/pull/2263">libp2p/go-libp2p#2263</a>)
webtransport: initialize the certmanager when creating the transport (<a href="https://redirect.github.com/libp2p/go-libp2p/pull/2268">libp2p/go-libp2p#2268</a>)</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/libp2p/go-libp2p/blob/master/CHANGELOG.md">github.com/libp2p/go-libp2p's changelog</a>.</em></p>
<blockquote>
<h1>Table Of Contents <!-- raw HTML omitted --></h1>
<ul>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0280">v0.28.0</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0270">v0.27.0</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0264">v0.26.4</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0263">v0.26.3</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0262">v0.26.2</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0261">v0.26.1</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0260">v0.26.0</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0251">v0.25.1</a></li>
<li><a href="https://github.com/libp2p/go-libp2p/blob/master/#v0250">v0.25.0</a></li>
</ul>
<h1><a href="https://github.com/libp2p/go-libp2p/releases/tag/v0.28.0">v0.28.0</a></h1>
<h2>🔦 Highlights <!-- raw HTML omitted --></h2>
<h3>Smart Dialing <!-- raw HTML omitted --></h3>
<p>This release introduces smart dialing logic. Currently, libp2p dials all addresses of a remote peer in parallel, and
aborts all outstanding dials as soon as the first one succeeds.
Dialing many addresses in parallel creates a lot of churn on the client side, and unnecessary load on the network and
on the server side, and is heavily discouraged by the networking community (see <a href="https://www.rfc-editor.org/rfc/rfc8305">RFC 8305</a> for example).</p>
<p>When connecting to a peer we first determine the order to dial its addresses. This ranking logic considers a number of corner cases
described in detail in the documentation of the swarm package (<code>swarm.DefaultDialRanker</code>).
At a high level, this is what happens:</p>
<ul>
<li>If a peer offers a WebTransport and a QUIC address (on the same IP:port), the QUIC address is preferred.</li>
<li>If a peer has a QUIC and a TCP address, the QUIC address is dialed first. Only if the connection attempt doesn't succeed within 250ms, a TCP connection is started.</li>
</ul>
<p>Our measurements on the IPFS network show that for &gt;90% of established libp2p connections, the first connection attempt succeeds,
leading a dramatic decrease in the number of aborted connection attempts.</p>
<p>We also added new metrics to the swarm Grafana dashboard, showing:</p>
<ul>
<li>The number of connection attempts it took to establish a connection</li>
<li>The delay introduced by the ranking logic</li>
</ul>
<p>This feature should be safe to enable for nodes running in data centers and for most nodes in home networks.
However, there are some (mostly home and corporate networks) that block all UDP traffic. If enabled, the current implementation
of the smart dialing logic will lead to a regression, since it preferes QUIC addresses over TCP addresses. Nodes would still be
able to connect, but connection establishment of the TCP connection would be delayed by 250ms.</p>
<p>In a future release (see <a href="https://redirect.github.com/libp2p/go-libp2p/issues/1605">#1605</a> for details), we will introduce a feature called blackhole detection. By observing the outcome of
QUIC connection attempts, we can determine if UDP traffic is blocked (namely, if all QUIC connection attempts fail), and stop
dialing QUIC in this case altogether. Once this detection logic is in place, smart dialing will be enabled by default.</p>
<h3>More Metrics! <!-- raw HTML omitted --></h3>
<p>Since the last release, we've added metrics for:</p>
<ul>
<li><a href="https://redirect.github.com/libp2p/go-libp2p/pull/2246">Holepunching</a></li>
<li>Smart Dialing (see above)</li>
</ul>
<h3>WebTransport <!-- raw HTML omitted --></h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/libp2p/go-libp2p/commit/8506ab233441d434bb777615fffefab64b06f335"><code>8506ab2</code></a> release v0.27.8</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/69acf8bd0714c73148adee729b39d3a996423de3"><code>69acf8b</code></a> swarm: don't open new streams over transient connections (<a href="https://redirect.github.com/libp2p/go-libp2p/issues/2450">#2450</a>)</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/b7ebfaaf4fa133a9e2587809467726b7965e2964"><code>b7ebfaa</code></a> manually bump qtls dependencies to fix RSA key size vulnerability</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/0cce607219f3710addc7e18672cffd1f1d912fbb"><code>0cce607</code></a> core/crypto: restrict RSA keys to &lt;= 8192 bits (<a href="https://redirect.github.com/libp2p/go-libp2p/issues/2454">#2454</a>)</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/68ad5ea717cc48f6d9732ba7fa4c0dff68854a5d"><code>68ad5ea</code></a> Release v0.27.7 (<a href="https://redirect.github.com/libp2p/go-libp2p/issues/2374">#2374</a>)</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/2df518f43fa2c3e937b81c249c2c5b898421df6b"><code>2df518f</code></a> Release v0.27.6 (<a href="https://redirect.github.com/libp2p/go-libp2p/issues/2359">#2359</a>)</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/6dffa1a946874ab63f79a28ad85c11fa373cb69d"><code>6dffa1a</code></a> Release v0.27.5 (<a href="https://redirect.github.com/libp2p/go-libp2p/issues/2324">#2324</a>)</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/fc89448282cf623011805ed35fd27ee392b2f019"><code>fc89448</code></a> Bump version to v0.27.4</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/45d3c6fff662ddd6938982e7e9309ad5fa2ad8dd"><code>45d3c6f</code></a> identify: reject signed peer records on peer ID mismatch</li>
<li><a href="https://github.com/libp2p/go-libp2p/commit/40978ee08bc99999366638cbc8ee4934e7c437e8"><code>40978ee</code></a> swarm: change maps with multiaddress keys to use strings (<a href="https://redirect.github.com/libp2p/go-libp2p/issues/2284">#2284</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/libp2p/go-libp2p/compare/v0.26.4...v0.27.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/libp2p/go-libp2p&package-manager=go_modules&previous-version=0.26.4&new-version=0.27.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 13:23:51 +0000 UTC
    </div>
</div>

