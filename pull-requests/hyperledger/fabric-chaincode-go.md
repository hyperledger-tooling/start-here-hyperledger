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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/42" class=".btn">#42</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.23.0 to 1.46.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.23.0 to 1.46.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
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
<h1>Bug Fixes</h1>
<ul>
<li>metadata: make a copy of the value slices in FromContext() functions so that modifications won't be made to the original copy (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5267">#5267</a>)</li>
<li>client: handle invalid service configs by applying the default, if applicable (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5238">#5238</a>)</li>
<li>xds: the xds client will now apply a 1 second backoff before recreating ADS or LRS streams (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5280">#5280</a>)</li>
</ul>
<h1>Dependencies</h1>
<ul>
<li>Upgrade security/authorization module dependencies to <a href="https://github.com/google/cel-go">https://github.com/google/cel-go</a> v0.10.1 and others (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5243">#5243</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/TristonianJones"><code>@​TristonianJones</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.45.0</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds/clusterresolver: pass cluster name to DNS child policy to be used in creds handshake (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5119">#5119</a>)</li>
<li>reflection: support dynamic messages (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5180">#5180</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/codebutler"><code>@​codebutler</code></a></li>
</ul>
</li>
</ul>
<h1>Performance Improvements</h1>
<ul>
<li>wrr: improve randomWRR performance (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5067">#5067</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/huangchong94"><code>@​huangchong94</code></a></li>
</ul>
</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>server: convert context errors returned by service handlers to status with the correct status code (<code>Canceled</code> or <code>DeadlineExceeded</code>), instead of <code>Unknown</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5156">#5156</a>)</li>
</ul>
<h1>New Features</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/e8d06c51a523ba75f052cfaa56a1b8e0583ac589"><code>e8d06c5</code></a> Change version to 1.46.0 (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5296">#5296</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/efbd542a4f9947d6b1392f538e3b0dd3d1c94b90"><code>efbd542</code></a> gcp/observability: correctly test this module in presubmit tests (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5300">#5300</a>) (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5307">#5307</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4467a29dbb390764f9792ce61af53017d621eb7c"><code>4467a29</code></a> gcp/observability: implement logging via binarylog (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5196">#5196</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/18fdf542fab01f909e600763267ef13770a222d5"><code>18fdf54</code></a> cmd/protoc-gen-go-grpc: allow hooks to modify client structs and service hand...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/337b815c4150a12d15349cb9be5f22fb391918de"><code>337b815</code></a> interop: build client without timeout; add logs to help debug failures (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5294">#5294</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e583b196ce4717fdc024dd9432f8e4b229cc76e7"><code>e583b19</code></a> xds: Add RLS in xDS e2e test (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5281">#5281</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/0066bf69deb33b0e5bee4de69090c3ef8f6991aa"><code>0066bf6</code></a> grpc: perform graceful switching of LB policies in the <code>ClientConn</code> by defaul...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3cccf6a43b55b4a089e832213b0e34df859e1978"><code>3cccf6a</code></a> xdsclient: always backoff between new streams even after successful stream (#...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4e780933f85a4d0f6903d1a5bb57bb7c882e611d"><code>4e78093</code></a> xds: ignore routes with unsupported cluster specifiers (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5269">#5269</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/99aae3442dbe8495247dda07a6b1c8cda98accca"><code>99aae34</code></a> cluster manager: Add Graceful Switch functionality to Cluster Manager (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5265">#5265</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.23.0...v1.46.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.23.0&new-version=1.46.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-25 04:34:14 +0000 UTC
    </div>
</div>

