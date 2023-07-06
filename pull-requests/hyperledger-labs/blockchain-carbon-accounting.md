---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.7.0 to 1.8.17 in /fabric/chaincode/emissionscontract/typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.7.0 to 1.8.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.17</h2>
<ul>
<li>Disallow <code>pick_first</code> LB policy as the direct child of an <code>outlier_detection</code> LB policy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.16</h2>
<ul>
<li>Fix missing <code>transport</code> trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.15</h2>
<ul>
<li>Fix a memory leak that could result from a specific pattern of recursive function calls (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
<li>Ensure <code>status</code> and <code>error</code> events are consistently emitted asynchronously (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.14</h2>
<ul>
<li>Fix sequencing of some events related to connectivity state changes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2421">#2421</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.13</h2>
<ul>
<li>Fix memory leak in channelz socket tracking (<a href="https://redirect.github.com/grpc/grpc-node/issues/2394">#2394</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.12</h2>
<ul>
<li>Fix an occasional type error when receiving DNS updates (<a href="https://redirect.github.com/grpc/grpc-node/issues/2380">#2380</a>)</li>
<li>Fix ordering of events when handing requests on the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2376">#2376</a> contributed by <a href="https://github.com/phoenix741"><code>@​phoenix741</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.11</h2>
<ul>
<li>Avoid accumulating placeholder objects when sending many messages on a long-running stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2372">#2372</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.10</h2>
<ul>
<li>Fix bugs in &quot;pick first&quot; load balancing policy that caused incorrect reconnection behavior (<a href="https://redirect.github.com/grpc/grpc-node/issues/2369">#2369</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.9</h2>
<ul>
<li>Fix a bug where clients would continue to send pings at the original configured rate after receiving a backoff request from the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2363">#2363</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/409418b103f35c6b89371731e2b1d5084b442318"><code>409418b</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a> from murgatroid99/grpc-js_prohibit_od_pick_first</li>
<li><a href="https://github.com/grpc/grpc-node/commit/ed70a0b381144b387698f2d57001f5a7bc82cbe9"><code>ed70a0b</code></a> Fix handling of OD policy with no child</li>
<li><a href="https://github.com/grpc/grpc-node/commit/073caf5b83387be8c1c7416477489646060e4942"><code>073caf5</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2478">#2478</a> from murgatroid99/grpc-js-xds_docker_distroless_1.8.x</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d2d17b0b694d7c23e2448d9cde224b9427102fb4"><code>d2d17b0</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2482">#2482</a> from XuanWang-Amos/backport-1.8-file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a6aa7ea43e1458a578cf9ab81ed492a760c43a78"><code>a6aa7ea</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2475">#2475</a> from XuanWang-Amos/file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a62d2b027bf91e5084c9134305e88a645dc5f1c1"><code>a62d2b0</code></a> Use entrypoint /nodejs/bin/node</li>
<li><a href="https://github.com/grpc/grpc-node/commit/9441de78f655ada34ada0dc1a8057122eb21f229"><code>9441de7</code></a> grpc-js-xds: Use distroless Node image for interop Dockerfile</li>
<li><a href="https://github.com/grpc/grpc-node/commit/b53f5882f13a5cb3c599804e96304bf5b8407ea6"><code>b53f588</code></a> grpc-js: Disallow pick_first as child of outlier_detection</li>
<li><a href="https://github.com/grpc/grpc-node/commit/09d74ca43d2fcb63c97405315bd01633322d9b34"><code>09d74ca</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a> from murgatroid99/grpc-js_transport_trace_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/87b5466b1b5e6d269a9750305c5842c9e30e56e8"><code>87b5466</code></a> grpc-js: Implement trace function in Http2SubchannelConnector</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.7.0...@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.7.0&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 23:26:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.6.8 to 1.8.17 in /fabric/docker-compose-setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.6.8 to 1.8.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.17</h2>
<ul>
<li>Disallow <code>pick_first</code> LB policy as the direct child of an <code>outlier_detection</code> LB policy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.16</h2>
<ul>
<li>Fix missing <code>transport</code> trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.15</h2>
<ul>
<li>Fix a memory leak that could result from a specific pattern of recursive function calls (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
<li>Ensure <code>status</code> and <code>error</code> events are consistently emitted asynchronously (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.14</h2>
<ul>
<li>Fix sequencing of some events related to connectivity state changes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2421">#2421</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.13</h2>
<ul>
<li>Fix memory leak in channelz socket tracking (<a href="https://redirect.github.com/grpc/grpc-node/issues/2394">#2394</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.12</h2>
<ul>
<li>Fix an occasional type error when receiving DNS updates (<a href="https://redirect.github.com/grpc/grpc-node/issues/2380">#2380</a>)</li>
<li>Fix ordering of events when handing requests on the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2376">#2376</a> contributed by <a href="https://github.com/phoenix741"><code>@​phoenix741</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.11</h2>
<ul>
<li>Avoid accumulating placeholder objects when sending many messages on a long-running stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2372">#2372</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.10</h2>
<ul>
<li>Fix bugs in &quot;pick first&quot; load balancing policy that caused incorrect reconnection behavior (<a href="https://redirect.github.com/grpc/grpc-node/issues/2369">#2369</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.9</h2>
<ul>
<li>Fix a bug where clients would continue to send pings at the original configured rate after receiving a backoff request from the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2363">#2363</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/grpc/grpc-node/commits/@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.6.8&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 23:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.6.7 to 1.8.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [@grpc/grpc-js](https://github.com/grpc/grpc-node) from 1.6.7 to 1.8.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.8.17</h2>
<ul>
<li>Disallow <code>pick_first</code> LB policy as the direct child of an <code>outlier_detection</code> LB policy (<a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.16</h2>
<ul>
<li>Fix missing <code>transport</code> trace logs (<a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.15</h2>
<ul>
<li>Fix a memory leak that could result from a specific pattern of recursive function calls (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
<li>Ensure <code>status</code> and <code>error</code> events are consistently emitted asynchronously (<a href="https://redirect.github.com/grpc/grpc-node/issues/2456">#2456</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.14</h2>
<ul>
<li>Fix sequencing of some events related to connectivity state changes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2421">#2421</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.13</h2>
<ul>
<li>Fix memory leak in channelz socket tracking (<a href="https://redirect.github.com/grpc/grpc-node/issues/2394">#2394</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.12</h2>
<ul>
<li>Fix an occasional type error when receiving DNS updates (<a href="https://redirect.github.com/grpc/grpc-node/issues/2380">#2380</a>)</li>
<li>Fix ordering of events when handing requests on the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2376">#2376</a> contributed by <a href="https://github.com/phoenix741"><code>@​phoenix741</code></a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.11</h2>
<ul>
<li>Avoid accumulating placeholder objects when sending many messages on a long-running stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2372">#2372</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.10</h2>
<ul>
<li>Fix bugs in &quot;pick first&quot; load balancing policy that caused incorrect reconnection behavior (<a href="https://redirect.github.com/grpc/grpc-node/issues/2369">#2369</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.9</h2>
<ul>
<li>Fix a bug where clients would continue to send pings at the original configured rate after receiving a backoff request from the server (<a href="https://redirect.github.com/grpc/grpc-node/issues/2363">#2363</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.8</h2>
<ul>
<li>Remove <code>progress</code> field in returned status object (<a href="https://redirect.github.com/grpc/grpc-node/issues/2350">#2350</a>)</li>
<li>Export <code>InterceptingListener</code> and <code>NextCall</code> types (<a href="https://redirect.github.com/grpc/grpc-node/issues/2351">#2351</a>)</li>
<li>Fix a bug that could cause a crash when sending messages that exceed the outgoing message buffer size while a retry is in progress (<a href="https://redirect.github.com/grpc/grpc-node/issues/2349">#2349</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.7</h2>
<ul>
<li>Make handling of HTTP2 session references work independent of keepalive settings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2337">#2337</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.6</h2>
<ul>
<li>Hold a reference to transport from call to avoid premature garbage collection (<a href="https://redirect.github.com/grpc/grpc-node/issues/2336">#2336</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.5</h2>
<ul>
<li>Cancel deadline timer when the call ends (<a href="https://redirect.github.com/grpc/grpc-node/issues/2335">#2335</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.4</h2>
<ul>
<li>Fix a bug that would sometimes allow the Node process to exit even though a gRPC request is active (<a href="https://redirect.github.com/grpc/grpc-node/issues/2322">#2322</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.8.3</h2>
<ul>
<li>Fix bug that caused streams to fail early when receiving a GOAWAY (<a href="https://redirect.github.com/grpc/grpc-node/issues/2319">#2319</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code><a href="https://github.com/1"><code>@​1</code></a>.8.2</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/409418b103f35c6b89371731e2b1d5084b442318"><code>409418b</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2476">#2476</a> from murgatroid99/grpc-js_prohibit_od_pick_first</li>
<li><a href="https://github.com/grpc/grpc-node/commit/ed70a0b381144b387698f2d57001f5a7bc82cbe9"><code>ed70a0b</code></a> Fix handling of OD policy with no child</li>
<li><a href="https://github.com/grpc/grpc-node/commit/073caf5b83387be8c1c7416477489646060e4942"><code>073caf5</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2478">#2478</a> from murgatroid99/grpc-js-xds_docker_distroless_1.8.x</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d2d17b0b694d7c23e2448d9cde224b9427102fb4"><code>d2d17b0</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2482">#2482</a> from XuanWang-Amos/backport-1.8-file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a6aa7ea43e1458a578cf9ab81ed492a760c43a78"><code>a6aa7ea</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2475">#2475</a> from XuanWang-Amos/file_multiple_url_map</li>
<li><a href="https://github.com/grpc/grpc-node/commit/a62d2b027bf91e5084c9134305e88a645dc5f1c1"><code>a62d2b0</code></a> Use entrypoint /nodejs/bin/node</li>
<li><a href="https://github.com/grpc/grpc-node/commit/9441de78f655ada34ada0dc1a8057122eb21f229"><code>9441de7</code></a> grpc-js-xds: Use distroless Node image for interop Dockerfile</li>
<li><a href="https://github.com/grpc/grpc-node/commit/b53f5882f13a5cb3c599804e96304bf5b8407ea6"><code>b53f588</code></a> grpc-js: Disallow pick_first as child of outlier_detection</li>
<li><a href="https://github.com/grpc/grpc-node/commit/09d74ca43d2fcb63c97405315bd01633322d9b34"><code>09d74ca</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2470">#2470</a> from murgatroid99/grpc-js_transport_trace_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/87b5466b1b5e6d269a9750305c5842c9e30e56e8"><code>87b5466</code></a> grpc-js: Implement trace function in Http2SubchannelConnector</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.6.7...@grpc/grpc-js@1.8.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=@grpc/grpc-js&package-manager=npm_and_yarn&previous-version=1.6.7&new-version=1.8.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 23:02:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.46.0 to 1.53.0 in /fabric/multi-cloud-deployment/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.46.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.46.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.46.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:20:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.46.0 to 1.53.0 in /fabric/chaincode/datalock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.46.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.46.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.46.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:19:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.46.0 to 1.53.0 in /fabric/multi-cloud-deployment/deploy-aws/chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.46.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.46.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.46.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Bump semver from 7.3.8 to 7.5.3 in /hardhat/hedera
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [semver](https://github.com/npm/node-semver) from 7.3.8 to 7.5.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/releases">semver's releases</a>.</em></p>
<blockquote>
<h2>v7.5.3</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2>v7.5.2</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2>v7.5.1</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2>v7.5.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2>v7.4.0</h2>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/113f51312a1a6b6aa50d4f9486b4fde21782c1f5"><code>113f513</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/532">#532</a> identifierBase parameter for .inc (<a href="https://redirect.github.com/npm/node-semver/issues/532">#532</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/b-bly"><code>@​b-bly</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/48d8f8fa63bf6e35db70ff840b6da1a51596a5a8"><code>48d8f8f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/530">#530</a> export new RELEASE_TYPES constant (<a href="https://github.com/hcharley"><code>@​hcharley</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/npm/node-semver/blob/main/CHANGELOG.md">semver's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.2...v7.5.3">7.5.3</a> (2023-06-22)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/571">#571</a> set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/569">#569</a> add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>) (<a href="https://github.com/mbtools"><code>@​mbtools</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.1...v7.5.2">7.5.2</a> (2023-06-15)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/566">#566</a> diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/565">#565</a> preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/564">#564</a> better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>) (<a href="https://github.com/lukekarrys"><code>@​lukekarrys</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.5.0...v7.5.1">7.5.1</a> (2023-05-12)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/559">#559</a> show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.4.0...v7.5.0">7.5.0</a> (2023-04-17)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/503a4e52fe2b1c6ed1400d33149f7733c8361eed"><code>503a4e5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/548">#548</a> allow identifierBase to be false (<a href="https://redirect.github.com/npm/node-semver/issues/548">#548</a>) (<a href="https://github.com/lsvalina"><code>@​lsvalina</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/e219bb454036a0c23e34407591f921c8edb688e7"><code>e219bb4</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/552">#552</a> throw on bad version with correct error message (<a href="https://redirect.github.com/npm/node-semver/issues/552">#552</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/fc2f3df0b5d25253b3580607e111a9a280d888ca"><code>fc2f3df</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/546">#546</a> incorrect results from diff sometimes with prerelease versions (<a href="https://redirect.github.com/npm/node-semver/issues/546">#546</a>) (<a href="https://github.com/tjenkinson"><code>@​tjenkinson</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/27817677794f592b592bf6181a80a4824ff762b2"><code>2781767</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/547">#547</a> avoid re-instantiating SemVer during diff compare (<a href="https://redirect.github.com/npm/node-semver/issues/547">#547</a>) (<a href="https://github.com/macno"><code>@​macno</code></a>)</li>
</ul>
<h2><a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.4.0">7.4.0</a> (2023-04-10)</h2>
<h3>Features</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/113f51312a1a6b6aa50d4f9486b4fde21782c1f5"><code>113f513</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/532">#532</a> identifierBase parameter for .inc (<a href="https://redirect.github.com/npm/node-semver/issues/532">#532</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/b-bly"><code>@​b-bly</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/48d8f8fa63bf6e35db70ff840b6da1a51596a5a8"><code>48d8f8f</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/530">#530</a> export new RELEASE_TYPES constant (<a href="https://github.com/hcharley"><code>@​hcharley</code></a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/940723d22bca824993627c45ac30dd3d2854b8cd"><code>940723d</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/538">#538</a> intersects with v0.0.0 and v0.0.0-0 (<a href="https://redirect.github.com/npm/node-semver/issues/538">#538</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/aa516b50b32f5a144017d8fc1b9efe0540963c91"><code>aa516b5</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/535">#535</a> faster parse options (<a href="https://redirect.github.com/npm/node-semver/issues/535">#535</a>) (<a href="https://github.com/H4ad"><code>@​H4ad</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/61e6ea1e9b7af01baf19ab0c0a63c8e3ebfac97c"><code>61e6ea1</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/536">#536</a> faster cache key factory for range (<a href="https://redirect.github.com/npm/node-semver/issues/536">#536</a>) (<a href="https://github.com/H4ad"><code>@​H4ad</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/f8b8b619e71746a47852a9d301f3087ab311444f"><code>f8b8b61</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/541">#541</a> optimistic parse (<a href="https://redirect.github.com/npm/node-semver/issues/541">#541</a>) (<a href="https://github.com/H4ad"><code>@​H4ad</code></a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/796cbe29b06d102e1b16f3ed78eaba210ece951e"><code>796cbe2</code></a> <a href="https://redirect.github.com/npm/node-semver/pull/533">#533</a> semver.diff prerelease to release recognition (<a href="https://redirect.github.com/npm/node-semver/issues/533">#533</a>) (<a href="https://github.com/wraithgar"><code>@​wraithgar</code></a>, <a href="https://github.com/dominique-blockchain"><code>@​dominique-blockchain</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-semver/commit/7fdf1ef223826b428d7f8aaf906e9eeefa9469f9"><code>7fdf1ef</code></a> chore: release 7.5.3</li>
<li><a href="https://github.com/npm/node-semver/commit/bf53dd8da15a17eb6b8111115d0d8ef341fea5db"><code>bf53dd8</code></a> docs: add example for <code>&gt;</code> comparator (<a href="https://redirect.github.com/npm/node-semver/issues/569">#569</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/abdd93d55496d22e3c15a454a5cf13f101e48bce"><code>abdd93d</code></a> fix: set max lengths in regex for numeric and build identifiers (<a href="https://redirect.github.com/npm/node-semver/issues/571">#571</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/e7b78de06eb14a7fa2075cedf9f167040d8d31af"><code>e7b78de</code></a> chore: release 7.5.2</li>
<li><a href="https://github.com/npm/node-semver/commit/58c791f40ba8cf4be35a5ca6644353ecd6249edc"><code>58c791f</code></a> fix: diff when detecting major change from prerelease (<a href="https://redirect.github.com/npm/node-semver/issues/566">#566</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/5c8efbcb3c6c125af10746d054faff13e8c33fbd"><code>5c8efbc</code></a> fix: preserve build in raw after inc (<a href="https://redirect.github.com/npm/node-semver/issues/565">#565</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/717534ee353682f3bcf33e60a8af4292626d4441"><code>717534e</code></a> fix: better handling of whitespace (<a href="https://redirect.github.com/npm/node-semver/issues/564">#564</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/2f738e9a70d9b9468b7b69e9ed3e12418725c650"><code>2f738e9</code></a> chore: bump <code>@​npmcli/template-oss</code> from 4.14.1 to 4.15.1 (<a href="https://redirect.github.com/npm/node-semver/issues/558">#558</a>)</li>
<li><a href="https://github.com/npm/node-semver/commit/aa016a67162c195938f7873ea29a73dac47ff9ba"><code>aa016a6</code></a> chore: release 7.5.1</li>
<li><a href="https://github.com/npm/node-semver/commit/d30d25a5c1fb963c3cc9178cb1769fe45e4a3cab"><code>d30d25a</code></a> fix: show type on invalid semver error (<a href="https://redirect.github.com/npm/node-semver/issues/559">#559</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-semver/compare/v7.3.8...v7.5.3">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~npm-cli-ops">npm-cli-ops</a>, a new releaser for semver since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=semver&package-manager=npm_and_yarn&previous-version=7.3.8&new-version=7.5.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-01 02:41:34 +0000 UTC
    </div>
</div>

