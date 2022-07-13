---
layout: default
title: fabric-chaincode-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-go
---

# fabric-chaincode-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.23.0 to 1.48.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.23.0 to 1.48.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.48.0</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds/priority: fix bug that could prevent higher priorities from receiving config updates (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5417">#5417</a>)</li>
<li>RLS load balancer: don't propagate the status code returned on control plane RPCs to data plane RPCs (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5400">#5400</a>)</li>
</ul>
<h1>New Features</h1>
<ul>
<li>stats: add support for multiple stats handlers in a single client or server (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5347">#5347</a>)</li>
<li>gcp/observability: add experimental OpenCensus tracing/metrics support (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5372">#5372</a>)</li>
<li>xds: enable aggregate and logical DNS clusters by default (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5380">#5380</a>)</li>
<li>credentials/google (for xds): support xdstp C2P cluster names (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5399">#5399</a>)</li>
</ul>
<h2>Release 1.47.0</h2>
<h1>New Features</h1>
<ul>
<li>xds: add support for RBAC metadata invert matchers (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5345">#5345</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>client: fix a context leaked if a connection to an address is lost before it is fully established (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5337">#5337</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/carzil"><code>@​carzil</code></a></li>
</ul>
</li>
<li>client: fix potential panic during RPC retries (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5323">#5323</a>)</li>
<li>xds/client: fix a potential concurrent map read/write in load reporting (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5331">#5331</a>)</li>
<li>client/SubConn: do not recreate addrConn if UpdateAddresses is called with the same addresses (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5373">#5373</a>)</li>
<li>xds/eds: resources containing duplicate localities with the same priority will be rejected (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5303">#5303</a>)</li>
<li>server: return Canceled or DeadlineExceeded status code when writing headers to a stream that is already closed (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5292">#5292</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/idiamond-stripe"><code>@​idiamond-stripe</code></a></li>
</ul>
</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>xds/priority: start the init timer when a child switches to Connecting from non-failure states (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5334">#5334</a>)</li>
<li>server: respond with HTTP Status 405 and gRPC status INTERNAL if the method sent to server is not POST (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5364">#5364</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>server: clarify documentation around setting and sending headers and ServerStream errors (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5302">#5302</a>)</li>
</ul>
<h2>Release v1.46.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>client: fix potential panic during RPC retries (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5323">#5323</a>)</li>
<li>xds: fix leak of deleted CDS resources from CSDS view (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5339">#5339</a>)</li>
</ul>
<h2>Release 1.46.0</h2>
<h1>New Features</h1>
<ul>
<li>server: Support setting <code>TCP_USER_TIMEOUT</code> on <code>grpc.Server</code> connections using <code>keepalive.ServerParameters.Time</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5219">#5219</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/bonnefoa"><code>@​bonnefoa</code></a></li>
</ul>
</li>
<li>client: perform graceful switching of LB policies in the <code>ClientConn</code> by default (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5285">#5285</a>)</li>
<li>all: improve logging by including channelz identifier in log messages (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5192">#5192</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/64174955202ffb5ea4122e25d1aaece49cc5a3ed"><code>6417495</code></a> Change version to 1.48.0 (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5482">#5482</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/5770b1dea58dd6a8bddb0585e40ed63d4d096e27"><code>5770b1d</code></a> xds: drop localities with zero weight at the xdsClient layer (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5476">#5476</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/423cd8e3ad5ff82dee28390f6fecd0e8658b4cd8"><code>423cd8e</code></a> interop: update proto to make vet happy (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5475">#5475</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c9b16c884c9797f5cdde9c2aeba2c20320213cd6"><code>c9b16c8</code></a> transport: remove unused <code>bufWriter.onFlush()</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5464">#5464</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/755bf5a191a0c1fd427c0794121dac58475f080e"><code>755bf5a</code></a> fix typo in the binary log (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5467">#5467</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/15739b5c88737e866194c45328750deb3521ab83"><code>15739b5</code></a> health: split imports into healthpb and healthgrpc (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5466">#5466</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c075d2011c8b55585404b52c1d358e0cbb39c355"><code>c075d20</code></a> interop client: provide new flag, --soak_min_time_ms_between_rpcs (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5421">#5421</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4b750055a530f53ee3715fe6763bf8855677847b"><code>4b75005</code></a> clusterresolver: merge P(p)arseConfig functions (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5462">#5462</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d883f3d5faf91e030539ce310875850357c6c4a8"><code>d883f3d</code></a> test/xds: fail only when state changes to something other than READY and IDLE...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c6ee1c71447e2e5a1bbb017f6162a1840fb2e2c6"><code>c6ee1c7</code></a> xdsclient: only include nodeID in error strings, not the whole nodeProto (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5461">#5461</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.23.0...v1.48.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.23.0&new-version=1.48.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 04:36:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 17:39:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Add PurgePrivateData to ChaincodeStubInterface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Required to complete #44

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 16:05:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Remove azure pipelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 15:26:56 +0000 UTC
    </div>
</div>

