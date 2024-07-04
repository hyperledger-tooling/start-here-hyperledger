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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Change go.mod to 1.21.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update go.mod files to use toolchain compatible full version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 13:54:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.64.0 to 1.65.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.64.0 to 1.65.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.65.0</h2>
<h1>Dependencies</h1>
<ul>
<li>Change support policy to cover only the latest TWO releases of Go, matching the policy for Go itself.  See <a href="https://redirect.github.com/grpc/grpc-go/issues/7249">#7249</a> for more information. (<a href="https://redirect.github.com/grpc/grpc-go/issues/7250">#7250</a>)</li>
<li>Update x/net/http2 to address <a href="https://nvd.nist.gov/vuln/detail/CVE-2023-45288">CVE-2023-45288</a> (<a href="https://redirect.github.com/grpc/grpc-go/issues/7282">#7282</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>credentials/tls: clients and servers will now reject connections that don't support ALPN when environment variable <code>GRPC_ENFORCE_ALPN_ENABLED</code> is set to &quot;true&quot; (case insensitive). (<a href="https://redirect.github.com/grpc/grpc-go/issues/7184">#7184</a>)
<ul>
<li>NOTE: this behavior will become the default in a future release.</li>
</ul>
</li>
<li>metadata: remove String method from MD to make printing more consistent (<a href="https://redirect.github.com/grpc/grpc-go/issues/7373">#7373</a>)</li>
</ul>
<h1>New Features</h1>
<ul>
<li>grpc: add <code>WithMaxCallAttempts</code> to configure gRPC's retry behavior per-channel. (<a href="https://redirect.github.com/grpc/grpc-go/issues/7229">#7229</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/imoore76"><code>@​imoore76</code></a></li>
</ul>
</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>ringhash: properly apply endpoint weights instead of ignoring them (<a href="https://redirect.github.com/grpc/grpc-go/issues/7156">#7156</a>)</li>
<li>xds: fix a bug that could cause xds-enabled servers to stop accepting new connections after handshaking errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/7128">#7128</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/bozaro"><code>@​bozaro</code></a></li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/2da976983bbb33feb3e25b7daaa8f60b9769adb5"><code>2da9769</code></a> Change version to 1.65.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/7306">#7306</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ede96b776c9cea4ff2b06dfdedad841e53fb0c26"><code>ede96b7</code></a> metadata: remove String method (<a href="https://redirect.github.com/grpc/grpc-go/issues/7373">#7373</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/64be203f7828d03224aa44944a84deacac54b72b"><code>64be203</code></a> grpc: Readd pick first name (<a href="https://redirect.github.com/grpc/grpc-go/issues/7336">#7336</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7341">#7341</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/25e33a6c207464c6017d001255f9ac1297ba5d3e"><code>25e33a6</code></a> examples: Add CSM Observability example (<a href="https://redirect.github.com/grpc/grpc-go/issues/7302">#7302</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7318">#7318</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/04a5f4604baa9297b7168543834e531cfb8858dc"><code>04a5f46</code></a> xds/internal/xdsclient: Emit unknown for CSM Labels if not present in CDS (<a href="https://redirect.github.com/grpc/grpc-go/issues/7">#7</a>...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/cff5c3e3d0f104459af4f52e77fc1c49ef4cb6aa"><code>cff5c3e</code></a> stats/opentelemetry: Add e2e testing for CSM Observability (<a href="https://redirect.github.com/grpc/grpc-go/issues/7279">#7279</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7316">#7316</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/9b970fdd173c1951a354630133273639e8acf00c"><code>9b970fd</code></a> dns: fix constant 30s backoff for re-resolution (<a href="https://redirect.github.com/grpc/grpc-go/issues/7262">#7262</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7311">#7311</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6d236200ea68ea644d78a164c4ad9952a765aed3"><code>6d23620</code></a> documentation: on server, use FromIncomingContext  for retrieving context and...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/7e5898e7c569b8cc32d6eee9bc8ad1393a8fcc61"><code>7e5898e</code></a> xds: unify xDS client creation APIs meant for testing (<a href="https://redirect.github.com/grpc/grpc-go/issues/7268">#7268</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/5d7bd7aacb0c35fc14bf144fa81ecbb61eec91de"><code>5d7bd7a</code></a> interop/xds: Interop client and server changes for CSM Observability (<a href="https://redirect.github.com/grpc/grpc-go/issues/7280">#7280</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.64.0...v1.65.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.64.0&new-version=1.65.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 04:21:00 +0000 UTC
    </div>
</div>

