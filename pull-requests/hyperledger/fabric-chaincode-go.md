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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Bump github.com/golang/protobuf from 1.5.3 to 1.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/golang/protobuf](https://github.com/golang/protobuf) from 1.5.3 to 1.5.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/golang/protobuf/releases">github.com/golang/protobuf's releases</a>.</em></p>
<blockquote>
<h2>v1.5.4</h2>
<p>Notable changes</p>
<ul>
<li>update descriptor.proto to latest version</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/protobuf/commit/75de7c059e36b64f01d0dd234ff2fff404ec3374"><code>75de7c0</code></a> Merge pull request <a href="https://redirect.github.com/golang/protobuf/issues/1597">#1597</a> from golang/updatedesc</li>
<li><a href="https://github.com/golang/protobuf/commit/b7697bb698b1c56643249ef6179c7cae1478881d"><code>b7697bb</code></a> all: update descriptor.proto to latest version</li>
<li>See full diff in <a href="https://github.com/golang/protobuf/compare/v1.5.3...v1.5.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/golang/protobuf&package-manager=go_modules&previous-version=1.5.3&new-version=1.5.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-07 04:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.54.0 to 1.62.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.54.0 to 1.62.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
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
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/9952aa83979822b5915c3fcb2bb0f60afe55aa7d"><code>9952aa8</code></a> Change version to 1.62.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/7020">#7020</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d7334c477d1ea670fa8d5fa12f06a2bfe4f41d4f"><code>d7334c4</code></a> fix enabling compression by trimming whitespaces in accept encoding header (#...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d076e14b4849f4262f6f50042a9370ec5ce0116d"><code>d076e14</code></a> rpc_util: Fix RecvBufferPool deactivation issues (<a href="https://redirect.github.com/grpc/grpc-go/issues/6766">#6766</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/9d981b0eb01a1ccd61f16593461277e95e83a34b"><code>9d981b0</code></a> cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6997">#6997</a> to 1.62.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6979">#6979</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/7018">#7018</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/7c4b5533d07d5d7d01aa71145c32af27ac6e1a4d"><code>7c4b553</code></a> Switch version to 1.62.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6995">#6995</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d715b2ef0602fe2133221519cba0642ac282cc3f"><code>d715b2e</code></a> Change version to 1.62.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6994">#6994</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d706a42d29ab785cc1ad86a09fe828ef0a196f26"><code>d706a42</code></a> cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6926">#6926</a> to 1.62 release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6986">#6986</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/8a4ca0cc41ceb5bd0763c865cc4094650df9f95f"><code>8a4ca0c</code></a> cherry-pick <a href="https://redirect.github.com/grpc/grpc-go/issues/6977">#6977</a> to 1.62.x release branch (<a href="https://redirect.github.com/grpc/grpc-go/issues/6979">#6979</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d41b01db97ca2e3627b2c9949fffe8f152a4255d"><code>d41b01d</code></a> encoding: fix typo (<a href="https://redirect.github.com/grpc/grpc-go/issues/6966">#6966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/c2b50ee081682eca4b995d2fb79e642019f78aea"><code>c2b50ee</code></a> deps: fix backwards compatibility with encoding (<a href="https://redirect.github.com/grpc/grpc-go/issues/6965">#6965</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.54.0...v1.62.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.54.0&new-version=1.62.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-06 04:17:37 +0000 UTC
    </div>
</div>

