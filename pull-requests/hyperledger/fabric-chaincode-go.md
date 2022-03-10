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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/39" class=".btn">#39</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.23.0 to 1.45.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.23.0 to 1.45.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
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
<ul>
<li>reflection: add <code>NewServer(ServerOptions)</code> for creating a reflection server with advanced customizations (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5197">#5197</a>)</li>
<li>xds: support federation (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5128">#5128</a>)</li>
<li>xds/resource: accept Self as LDS's RDS config source and CDS's EDS config source (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5152">#5152</a>)</li>
<li>xds/bootstrap: add plugin system for credentials specified in bootstrap file (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5136">#5136</a>)</li>
</ul>
<h2>Release 1.44.0</h2>
<h1>New Features</h1>
<ul>
<li>balancer: add RLS load balancing policy (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5046">#5046</a>)</li>
<li>xds: add RLS Cluster Specifier Plugin (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5004">#5004</a>)</li>
<li>insecure: remove experimental notice (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5069">#5069</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>internal/balancergroup: eliminate race in exitIdle (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5012">#5012</a>)</li>
<li>authz: fix regex expression match (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5035">#5035</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>grpc: minor improvement on WithInsecure() document (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5068">#5068</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/shitian-ni"><code>@​shitian-ni</code></a></li>
</ul>
</li>
<li>attributes: document that some value types (e.g. <code>map</code>s) must implement Equal (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5109">#5109</a>)</li>
<li>dialoptions.go: Fix WithBlock godoc (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5073">#5073</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/sgreene570"><code>@​sgreene570</code></a></li>
</ul>
</li>
<li>grpclog.DepthLoggerV2: Correct comment: formats like fmt.Println (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5038">#5038</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/evanj"><code>@​evanj</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.43.0</h2>
<h1>API Changes</h1>
<ul>
<li>grpc: stabilize <code>WithConnectParams</code> <code>DialOption</code> (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/4915">#4915</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/a82cc96f07c960e02623688e4067ae6b7895334a"><code>a82cc96</code></a> Change version to 1.45.0 (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5202">#5202</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/011544f72939c85397b0e24378280e6075061cb1"><code>011544f</code></a> authz: add additional logs to sdk authz (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5094">#5094</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/18564ff61d5505d955c7bd1adc28e4f1ed96300c"><code>18564ff</code></a> reflection: improve server implementation (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5197">#5197</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ec717cad7395d45698b57c1df1ae36b4dbaa33dd"><code>ec717ca</code></a> xds: minor cleanup in xdsclient bootstrap code (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5195">#5195</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ebc30b8fc32e02f0ac5eff0ddbe4ccdca58bd8c4"><code>ebc30b8</code></a> reflection: use protobuf/reflect instead of go reflection, fix dynamic messag...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/46009ac902e2256a2675e6e7057d384f6fdc222d"><code>46009ac</code></a> transport: Add an Unwrap method to ConnectionError (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5148">#5148</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/75fd0240ac4146e5bcd211e0a3de695ad4369de3"><code>75fd024</code></a> remove sdk term from grpc authz (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5191">#5191</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a354b1eec35081ebfc7673a7edf273a13a2bfaee"><code>a354b1e</code></a> channelz: rename NewChannelzStorage to NewChannelzStorageForTesting (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5190">#5190</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/0e055491d58ccdd3cb7f30796559a20abfe8d505"><code>0e05549</code></a> Format directory/file references (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5184">#5184</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c44f627fd1f65c4e9f2837c17b4a734c516172fd"><code>c44f627</code></a> cleanup: replace grpc.WithInsecure with insecure.NewCredentials (<a href="https://github-redirect.dependabot.com/grpc/grpc-go/issues/5177">#5177</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.23.0...v1.45.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.23.0&new-version=1.45.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-10 04:34:39 +0000 UTC
    </div>
</div>

