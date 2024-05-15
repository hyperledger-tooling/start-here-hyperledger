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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.63.2 to 1.64.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.63.2 to 1.64.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.64.0</h2>
<h1>API Changes</h1>
<ul>
<li>stats: Deprecate <code>InPayload.Data</code> and <code>OutPayload.Data</code>; they were experimental and will be deleted in the next release (<a href="https://redirect.github.com/grpc/grpc-go/issues/7121">#7121</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>codec: Remove handling of environment variable <code>GRPC_GO_ADVERTISE_COMPRESSORS</code> to suppress setting supported compressors in <code>grpc-accept-encoding</code> header.  Compressors will always be advertised, as they have been by default for some time (<a href="https://redirect.github.com/grpc/grpc-go/issues/7203">#7203</a>)</li>
</ul>
<h1>New Features</h1>
<ul>
<li>resolver/dns: Add <code>SetMinResolutionInterval</code> to set the minimum interval at which DNS re-resolutions may occur (<a href="https://redirect.github.com/grpc/grpc-go/issues/6962">#6962</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/HomayoonAlimohammadi"><code>@​HomayoonAlimohammadi</code></a></li>
</ul>
</li>
<li>peer/peer: Implement the <code>fmt.Stringer</code> interface for pretty printing <code>Peer</code>, and</li>
<li>metadata/metadata: Implement the <code>fmt.Stringer</code> interface for pretty printing <code>MD</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/7137">#7137</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/AnomalRoil"><code>@​AnomalRoil</code></a></li>
</ul>
</li>
</ul>
<h1>Performance Improvements</h1>
<ul>
<li>client: Improve RPC performance by reducing work while holding a lock (<a href="https://redirect.github.com/grpc/grpc-go/issues/7132">#7132</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport/server: Display the proper timeout value when keepalive pings are not ack'd in time (<a href="https://redirect.github.com/grpc/grpc-go/issues/7038">#7038</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/BatmanAoD"><code>@​BatmanAoD</code></a></li>
</ul>
</li>
<li>channelz: Fix bug that was causing the subchannel's target to be unset (<a href="https://redirect.github.com/grpc/grpc-go/issues/7189">#7189</a>)</li>
<li>stats: Fix bug where peer was not set in context when calling stats handler for <code>OutPayload</code>, <code>InPayload</code>, and <code>End</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/7096">#7096</a>)</li>
</ul>
<h1>Dependencies</h1>
<ul>
<li>deps: Remove dependency on deprecated <code>github.com/golang/protobuf</code> module (<a href="https://redirect.github.com/grpc/grpc-go/issues/7122">#7122</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>grpc: Deprecate <code>WithBlock</code>, <code>WithReturnConnectionError</code>, <code>FailOnNonTempDialError</code> which are ignored by <code>NewClient</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/7097">#7097</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/pellared"><code>@​pellared</code></a></li>
</ul>
</li>
<li>grpc: Deprecate <code>Dial</code> and <code>DialContext</code>.  These will continue to be supported throughout 1.x, but are deprecated to direct users to <code>NewClient</code>  (See <a href="https://redirect.github.com/grpc/grpc-go/issues/7090">#7090</a> for more information)</li>
<li>examples: Add custom lb example (<a href="https://redirect.github.com/grpc/grpc-go/issues/6691">#6691</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/fa274d77904729c2893111ac292048d56dcf0bb1"><code>fa274d7</code></a> Change version to 1.64.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/7218">#7218</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6b413c8351abd92f8f9953bb9b41fc9e2262b99c"><code>6b413c8</code></a> xds: Surround two <code>Infof</code> calls that use <code>pretty.ToJSON</code> with <code>V(2)</code> checks (...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2dbbcefef2db79dcbe0ee25c1bdf040c4613ae9a"><code>2dbbcef</code></a> resolver/dns: Add docstring to SetMinResolutionInterval (<a href="https://redirect.github.com/grpc/grpc-go/issues/7217">#7217</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/070d9c793af46df05f24b4de548509627606f5b7"><code>070d9c7</code></a> codes: replace %q to %d in error string when invalid code is an integer (<a href="https://redirect.github.com/grpc/grpc-go/issues/7188">#7188</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/5d24ee2bd170a0c2c636b7d1ebc7ebdd3ecf81ac"><code>5d24ee2</code></a> xds: store server config for LRS server in xdsresource.ClusterUpdate (<a href="https://redirect.github.com/grpc/grpc-go/issues/7191">#7191</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c76f686c517261380b0a9a98d16510f271e4895e"><code>c76f686</code></a> advancedTLS: Rename get root certs related pieces (<a href="https://redirect.github.com/grpc/grpc-go/issues/7207">#7207</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/f591e3b82f76ee56ed32d53579332200242a10dc"><code>f591e3b</code></a> codec: remove option to suppress setting supported compressors in headers (<a href="https://redirect.github.com/grpc/grpc-go/issues/7">#7</a>...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/b4f7947184ed45e72283a37aeaf214e38c35bc63"><code>b4f7947</code></a> github: remove dependabot (<a href="https://redirect.github.com/grpc/grpc-go/issues/7208">#7208</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/0561c78c9dcb5876a140ff7be97f0f37abc36ec8"><code>0561c78</code></a> client: add user-friendly error message of LB policy update timed out (<a href="https://redirect.github.com/grpc/grpc-go/issues/7206">#7206</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/9d9c1fbd60cfd34608b731aa12a968d2f61a36d1"><code>9d9c1fb</code></a> peer: remove change detector test (<a href="https://redirect.github.com/grpc/grpc-go/issues/7204">#7204</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.63.2...v1.64.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.63.2&new-version=1.64.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-05-15 04:45:32 +0000 UTC
    </div>
</div>

