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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.54.0 to 1.63.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.54.0 to 1.63.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.63.0</h2>
<h1>Behavior Changes</h1>
<ul>
<li>grpc: Return canonical target string from <code>resolver.Address.String()</code> (experimental) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6923">#6923</a>)</li>
<li>client &amp; server: when using write buffer pooling, use input value for buffer size instead of size*2 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6983">#6983</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/raghav-stripe"><code>@​raghav-stripe</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>grpc: add <code>ClientConn.CanonicalTarget()</code> to return the canonical target string. (<a href="https://redirect.github.com/grpc/grpc-go/issues/7006">#7006</a>)</li>
<li>xds: implement LRS named metrics support (<a href="https://github.com/grpc/proposal/blob/master/A64-lrs-custom-metrics.md">gRFC A64</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7027">#7027</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/danielzhaotongliu"><code>@​danielzhaotongliu</code></a></li>
</ul>
</li>
<li>grpc: introduce <code>grpc.NewClient</code> to allow users to create new clients in idle mode and with &quot;dns&quot; as the default resolver (<a href="https://redirect.github.com/grpc/grpc-go/issues/7010">#7010</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/bruuuuuuuce"><code>@​bruuuuuuuce</code></a></li>
</ul>
</li>
</ul>
<h1>API Changes</h1>
<ul>
<li>grpc: stabilize experimental method <code>ClientConn.Target()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/7006">#7006</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix an issue that would cause the client to send an empty list of resources for LDS/CDS upon reconnecting with the management server (<a href="https://redirect.github.com/grpc/grpc-go/issues/7026">#7026</a>)</li>
<li>server: Fix some errors returned by a server when using a <code>grpc.Server</code> as an <code>http.Handler</code> with the Go stdlib HTTP server (<a href="https://redirect.github.com/grpc/grpc-go/issues/6989">#6989</a>)</li>
<li>resolver/dns: add <code>SetResolvingTimeout</code> to allow configuring the DNS resolver's global timeout (<a href="https://redirect.github.com/grpc/grpc-go/issues/6917">#6917</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/and1truong"><code>@​and1truong</code></a></li>
</ul>
</li>
<li>Set the security level of Windows named pipes to NoSecurity (<a href="https://redirect.github.com/grpc/grpc-go/issues/6956">#6956</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/irsl"><code>@​irsl</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.62.2</h2>
<h1>Dependencies</h1>
<ul>
<li>Update http2 library to address vulnerability <a href="https://www.kb.cert.org/vuls/id/421644">CVE-2023-45288</a></li>
</ul>
<h2>Release 1.62.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix a bug that results in <code>no matching virtual host found</code> RPC errors due to a difference between the target and LDS resource names (<a href="https://redirect.github.com/grpc/grpc-go/issues/6997">#6997</a>)</li>
<li>server: fixed stats handler data <code>InPayload.Length</code> for unary RPC calls (<a href="https://redirect.github.com/grpc/grpc-go/issues/6766">#6766</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/hueypark"><code>@​hueypark</code></a></li>
</ul>
</li>
<li>grpc: the experimental <code>RecvBufferPool</code> <code>DialOption</code> and <code>ServerOption</code> are now active during unary RPCs with compression (<a href="https://redirect.github.com/grpc/grpc-go/issues/6766">#6766</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/hueypark"><code>@​hueypark</code></a></li>
</ul>
</li>
<li>grpc: trim whitespaces in <code>accept-encoding</code> header before determining compressors
<ul>
<li>Special Thanks: <a href="https://github.com/sercand"><code>@​sercand</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.62.0</h2>
<h1>New Features</h1>
<ul>
<li>grpc: Add StaticMethod CallOption as a signal to stats handler that a method is safe to use as an instrument key (<a href="https://redirect.github.com/grpc/grpc-go/issues/6986">#6986</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/c68f4566b9cacdb11c42a6eb14ee66a33d9b7c12"><code>c68f456</code></a> Change version to 1.63.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/7050">#7050</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6369167ae33538aca051225fe5b5e07c2b022eb5"><code>6369167</code></a> *: update http2 dependency (<a href="https://redirect.github.com/grpc/grpc-go/issues/7082">#7082</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/88547614e7427f7ce87a5f5485d897ae09044641"><code>8854761</code></a> cherry-pick: channelz: fix race accessing channelMap without lock (<a href="https://redirect.github.com/grpc/grpc-go/issues/7079">#7079</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7">#7</a>...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e62770d76fc9508a2266d8bb8c6f2967e0dbc6fc"><code>e62770d</code></a> channelz: add LocalAddr to listen sockets and test (<a href="https://redirect.github.com/grpc/grpc-go/issues/7062">#7062</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7063">#7063</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4ffccf1a5f97417eeb000d521f6415b6eb33bb5f"><code>4ffccf1</code></a> googlec2p: use xdstp style template for client LDS resource name (<a href="https://redirect.github.com/grpc/grpc-go/issues/7048">#7048</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/faf9964afe47a919a1469419413a0cae4bc86769"><code>faf9964</code></a> gracefulswitch: add ParseConfig and make UpdateClientConnState call SwitchTo ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/800a8e02b5f25fa6aceb5771c0c263dae0928f8f"><code>800a8e0</code></a> channelz: re-add state for subchannels (<a href="https://redirect.github.com/grpc/grpc-go/issues/7046">#7046</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/dadbbfa2863a67ed640aac924b7b7fd18b50a429"><code>dadbbfa</code></a> channelz: re-add target and state (<a href="https://redirect.github.com/grpc/grpc-go/issues/7042">#7042</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/55cd7a68b3c18a0f76ea9c1be37221a5b901a798"><code>55cd7a6</code></a> channelz: major cleanup / reorganization (<a href="https://redirect.github.com/grpc/grpc-go/issues/6969">#6969</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a1033b1f44942fe30e3308ba85ee647e4187d97e"><code>a1033b1</code></a> xds: add LRS named metrics support (<a href="https://redirect.github.com/grpc/grpc-go/issues/7027">#7027</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.54.0...v1.63.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.54.0&new-version=1.63.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-04 04:58:41 +0000 UTC
    </div>
</div>

