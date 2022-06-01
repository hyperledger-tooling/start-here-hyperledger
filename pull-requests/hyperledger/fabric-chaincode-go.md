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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.23.0 to 1.47.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.23.0 to 1.47.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
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
<h1>API Changes</h1>
<ul>
<li>grpc: delete <code>WithBalancerName()</code> API, deprecated over 4 years ago in <a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/1697">#1697</a> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5232">#5232</a>)</li>
<li>balancer: change BuildOptions.ChannelzParentID to an opaque identifier instead of int (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5192">#5192</a>)
<ul>
<li>Note: the balancer package is labeled as EXPERIMENTAL, and we don't believe users were using this field.</li>
</ul>
</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>client: change connectivity state to <code>TransientFailure</code> in <code>pick_first</code> LB policy when all addresses are removed (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5274">#5274</a>)
<ul>
<li>This is a minor change that brings grpc-go's behavior in line with the intended behavior and how C and Java behave.</li>
</ul>
</li>
<li>metadata: add client-side validation of HTTP-invalid metadata before attempting to send (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4886">#4886</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/Patrick0308"><code>@​Patrick0308</code></a></li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/5b509df1e30a25b14dba119c09295924c9e17abe"><code>5b509df</code></a> Change version to 1.47.0 (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5377">#5377</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ed7522591b3485c919a04205094a07c2d96456ce"><code>ed75225</code></a> Don't call cmp in non testing file (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5370">#5370</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/081c688437c76dc60b2f6aec68c1804de5f32945"><code>081c688</code></a> client: fix hctx leakage in addrConn.createTransport (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5337">#5337</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/30b9d59a766858a4b51148e47edb3af2766ab617"><code>30b9d59</code></a> client/SubConn: do not recreate addrConn if UpdateAddresses is called with th...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/459729d6672eb555ada1060ceddf470ff8b1ec82"><code>459729d</code></a> xds/priority: avoid sending duplicate updates to children (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5374">#5374</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/9f4b31a11cc4deba7f5c542399d5ec71fab3a053"><code>9f4b31a</code></a> Added HTTP status and grpc status to POST check (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5364">#5364</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/333a441e27395b34f666e7d8f0ba871fae2ed53b"><code>333a441</code></a> xds/ringhash: update connectivity state aggregation, and make sure at least o...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e23132c6575e004c7ae416186d97d40057f0b928"><code>e23132c</code></a> Added support for metadata matcher invert (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5345">#5345</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d9b952b1706072a434320115194b98687bfeaffe"><code>d9b952b</code></a> xds/resolver: use correct resource name in log message (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5357">#5357</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/db79903af928ca8307700d83123a7702881c4e3c"><code>db79903</code></a> xds/priority: start the init timer when a child switch to Connecting from non...</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.23.0...v1.47.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.23.0&new-version=1.47.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-06-01 07:44:35 +0000 UTC
    </div>
</div>

