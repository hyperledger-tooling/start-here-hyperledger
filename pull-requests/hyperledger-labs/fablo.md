---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    Bump @grpc/grpc-js from 1.6.7 to 1.8.17 in /samples/chaincodes/chaincode-kv-node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fablo/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 23:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                     Fix NPM issues causing errors 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes some issues caused by npm by:

- Removing unsupported test library for fabric that depends on packages that fail to compile 
- Bumps nodejs version from 12 to 16 at `samples/chaincodes/chaincode-kv-node/.nvmrc`
- Removing non-crucial tests from the sample chaincode 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 22:16:38 +0000 UTC
    </div>
</div>

