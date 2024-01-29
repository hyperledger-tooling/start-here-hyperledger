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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.54.0 to 1.61.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.54.0 to 1.61.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.61.0</h2>
<h1>New Features</h1>
<ul>
<li>resolver: provide method, <code>AuthorityOverrider</code>, to allow resolver.Builders to override the default authority for a <code>ClientConn</code>. (EXPERIMENTAL) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6752">#6752</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/Aditya-Sood"><code>@​Aditya-Sood</code></a></li>
</ul>
</li>
<li>xds: add support for mTLS Credentials in xDS bootstrap (<a href="https://github.com/grpc/grpc-go/blob/HEAD/github.com/grpc/proposal/blob/8c31bfedded5f0a51c4933e9e9a8246122f9c41a/A65-xds-mtls-creds-in-bootstrap.md">gRFC A65</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6757">#6757</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/atollena"><code>@​atollena</code></a></li>
</ul>
</li>
<li>server: add <code>grpc.WaitForHandlers</code> <code>ServerOption</code> to cause <code>Server.Stop</code> to block until method handlers return. (EXPERIMENTAL)  (<a href="https://redirect.github.com/grpc/grpc-go/issues/6922">#6922</a>)</li>
</ul>
<h1>Performance Improvements</h1>
<ul>
<li>grpc: skip compression of empty messages as an optimization (<a href="https://redirect.github.com/grpc/grpc-go/issues/6842">#6842</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/jroper"><code>@​jroper</code></a></li>
</ul>
</li>
<li>orca: use atomic pointer to improve performance in server metrics recorder (<a href="https://redirect.github.com/grpc/grpc-go/issues/6799">#6799</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/danielzhaotongliu"><code>@​danielzhaotongliu</code></a></li>
</ul>
</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>client: correctly enable TCP keepalives with OS defaults on windows (<a href="https://redirect.github.com/grpc/grpc-go/issues/6863">#6863</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/mmatczuk"><code>@​mmatczuk</code></a></li>
</ul>
</li>
<li>server: change some stream operations to return <code>UNAVAILABLE</code> instead of <code>UNKNOWN</code> when underlying connection is broken (<a href="https://redirect.github.com/grpc/grpc-go/issues/6891">#6891</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/mustafasen81"><code>@​mustafasen81</code></a></li>
</ul>
</li>
<li>server: fix <code>GracefulStop</code> to block until all method handlers return (v1.60 regression). (<a href="https://redirect.github.com/grpc/grpc-go/issues/6922">#6922</a>)</li>
<li>server: fix two bugs that could lead to panics at shutdown when using <a href="https://pkg.go.dev/google.golang.org/grpc#NumStreamWorkers"><code>NumStreamWorkers</code></a> (EXPERIMENTAL). (<a href="https://redirect.github.com/grpc/grpc-go/issues/6856">#6856</a>)</li>
<li>reflection: do not send invalid descriptors to clients for files that cannot be fully resolved (<a href="https://redirect.github.com/grpc/grpc-go/issues/6771">#6771</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/jhump"><code>@​jhump</code></a></li>
</ul>
</li>
<li>xds: don't fail channel/server startup when xds creds is specified, but bootstrap is missing certificate providers (<a href="https://redirect.github.com/grpc/grpc-go/issues/6848">#6848</a>)</li>
<li>xds: Atomically read and write xDS security configuration client side (<a href="https://redirect.github.com/grpc/grpc-go/issues/6796">#6796</a>)</li>
<li>xds/server: fix RDS handling for non-inline route configs (<a href="https://redirect.github.com/grpc/grpc-go/issues/6915">#6915</a>)</li>
</ul>
<h2>Release v1.60.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>server: fix two bugs that could lead to panics at shutdown when using <a href="https://pkg.go.dev/google.golang.org/grpc#NumStreamWorkers">NumStreamWorkers</a> (experimental feature).</li>
</ul>
<h2>Release 1.60.0</h2>
<h1>Security</h1>
<ul>
<li>credentials/tls: if not set, set TLS MinVersion to 1.2 and CipherSuites according to supported suites not forbidden by RFC7540.
<ul>
<li>This is a behavior change to bring us into better alignment with RFC 7540.</li>
</ul>
</li>
</ul>
<h1>API Changes</h1>
<ul>
<li>resolver: remove deprecated and experimental <code>ClientConn.NewServiceConfig</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6784">#6784</a>)</li>
<li>client: remove deprecated <code>grpc.WithServiceConfig</code> <code>DialOption</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6800">#6800</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/8167bc3aca7890b44b5839a2cd92d495016ac7ed"><code>8167bc3</code></a> Change version to 1.61.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6936">#6936</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52e23632fc29be90369d5d479f8b4f752f4b1dc4"><code>52e2363</code></a> test/xds: Use different import path for gRPC Messages (<a href="https://redirect.github.com/grpc/grpc-go/issues/6933">#6933</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/67e50be52699e793bc89a786465e841a18950fae"><code>67e50be</code></a> transport: Remove redundant if in handleGoAway (<a href="https://redirect.github.com/grpc/grpc-go/issues/6930">#6930</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e96f521f478253ceb7d06c0282775e86223b5225"><code>e96f521</code></a> alts: Extract AuthInfo after handshake in ALTS e2e test. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6931">#6931</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/987df1309236a950d3f618eb5287279d81a7396e"><code>987df13</code></a> metadata: move FromOutgoingContextRaw() to internal (<a href="https://redirect.github.com/grpc/grpc-go/issues/6765">#6765</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/61eab37838ce213237ecb31aa7cdf95241851431"><code>61eab37</code></a> server: block GracefulStop on method handlers and make blocking optional for ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ddd377f19841eae70862559c854d957d61b3b692"><code>ddd377f</code></a> xds/server: fix RDS handling for non-inline route configs (<a href="https://redirect.github.com/grpc/grpc-go/issues/6915">#6915</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8b455deef5597ea1d5af9b168028bc8a087a0e8c"><code>8b455de</code></a> removing Roots deprecated Subjects field in tests (<a href="https://redirect.github.com/grpc/grpc-go/issues/6907">#6907</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/953d12a1c6c5b4929ac92eeeedfdad2ddef49976"><code>953d12a</code></a> alts: Forward-fix of ALTS queuing of handshake requests. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6906">#6906</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6ce73bfbf9c5ca458c346f62c571a3a74369c4c4"><code>6ce73bf</code></a> internal/transport: convert <code>ConnectionError</code> to <code>Unavailable</code> status when wr...</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.54.0...v1.61.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.54.0&new-version=1.61.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-01-24 04:16:30 +0000 UTC
    </div>
</div>

