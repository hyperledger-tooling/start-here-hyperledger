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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.54.0 to 1.62.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.54.0 to 1.62.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.62.0</h2>
<h1>New Features</h1>
<ul>
<li>grpc: Add StaticMethod CallOption as a signal to stats handler that a method is safe to use as an instrument key (<a href="https://redirect.github.com/grpc/grpc-go/issues/6986">#6986</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<ul>
<li>grpc: Return canonical target string from ClientConn.Target() and resolver.Address.String() (<a href="https://redirect.github.com/grpc/grpc-go/issues/6923">#6923</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>server: wait to close connection until incoming socket is drained (with timeout) to prevent data loss on client-side (<a href="https://redirect.github.com/grpc/grpc-go/issues/6977">#6977</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/s-matyukevich"><code>@​s-matyukevich</code></a> for discovering the root cause</li>
</ul>
</li>
</ul>
<h1>Performance Improvements</h1>
<ul>
<li>*: Allow building without <code>x/net/trace</code> by using <code>grpcnotrace</code> to enable dead code elimination (<a href="https://redirect.github.com/grpc/grpc-go/issues/6954">#6954</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/hugelgupf"><code>@​hugelgupf</code></a></li>
</ul>
</li>
<li>rand: improve performance and simplify implementation of <code>grpcrand</code> by adopting <code>math/rand</code>'s top-level functions for go version 1.21.0 and newer. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6925">#6925</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kmirzavaziri"><code>@​kmirzavaziri</code></a></li>
</ul>
</li>
</ul>
<h1>Dependencies</h1>
<ul>
<li>*: Use google.golang.org/protobuf/proto instead of github.com/golang/protobuf. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6919">#6919</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/Clement-Jean"><code>@​Clement-Jean</code></a></li>
</ul>
</li>
</ul>
<blockquote>
<p>[!NOTE]
The above change in proto library usage introduces a minor behavior change within those libraries.  The old <code>github.com/golang/protobuf</code> library would error if given a <code>nil</code> message to <code>Marshal</code>, while the new <code>google.golang.org/protobuf</code> library will successfully output zero bytes in this case.  This means server method handlers that did <code>return nil, nil</code> will now return an empty message and no error, while it used to return an error.  This also affects the client side, where clients sending <code>nil</code> messages used to fail without sending the RPC, and now they will send an empty message.</p>
</blockquote>
<h2>Release 1.61.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>server: wait to close connection until incoming socket is drained (with timeout) to prevent data loss on client-side (<a href="https://redirect.github.com/grpc/grpc-go/issues/6977">#6977</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/s-matyukevich"><code>@​s-matyukevich</code></a> for discovering the root cause</li>
</ul>
</li>
</ul>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/d715b2ef0602fe2133221519cba0642ac282cc3f"><code>d715b2e</code></a> Change version to 1.62.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6994">#6994</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d706a42d29ab785cc1ad86a09fe828ef0a196f26"><code>d706a42</code></a> cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6926">#6926</a> to 1.62 release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6986">#6986</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8a4ca0cc41ceb5bd0763c865cc4094650df9f95f"><code>8a4ca0c</code></a> cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6977">#6977</a> to 1.62.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6979">#6979</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d41b01db97ca2e3627b2c9949fffe8f152a4255d"><code>d41b01d</code></a> encoding: fix typo (<a href="https://redirect.github.com/grpc/grpc-go/issues/6966">#6966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c2b50ee081682eca4b995d2fb79e642019f78aea"><code>c2b50ee</code></a> deps: fix backwards compatibility with encoding (<a href="https://redirect.github.com/grpc/grpc-go/issues/6965">#6965</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/05b4a8b8f779518bb0119042c8c5806fa33d2184"><code>05b4a8b</code></a> Revert &quot;xds/googlec2p: use xdstp names for LDS (<a href="https://redirect.github.com/grpc/grpc-go/issues/6949">#6949</a>)&quot; (<a href="https://redirect.github.com/grpc/grpc-go/issues/6964">#6964</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/03e76b3d2a467a6deebabe2b323780a1890e36d4"><code>03e76b3</code></a> grpc: add ability to compile with or without tracing (<a href="https://redirect.github.com/grpc/grpc-go/issues/6954">#6954</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/84b85babc00b4b8460e53b6ee110bfb49e9311cf"><code>84b85ba</code></a> xds/googledirectpath: Check if ipv6 address is non empty (<a href="https://redirect.github.com/grpc/grpc-go/issues/6959">#6959</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6f63f05a5b98c484020c143d69450e8679603953"><code>6f63f05</code></a> internal/grpcrand: use Go top-level random functions for go1.21+ (<a href="https://redirect.github.com/grpc/grpc-go/issues/6925">#6925</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/cd69b5d0af6bd46ca17b94acaa09256a863ac277"><code>cd69b5d</code></a> .*: fix minor linter issues (<a href="https://redirect.github.com/grpc/grpc-go/issues/6958">#6958</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.54.0...v1.62.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.54.0&new-version=1.62.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-22 05:02:28 +0000 UTC
    </div>
</div>

