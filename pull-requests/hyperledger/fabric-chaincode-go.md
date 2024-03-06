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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Bump github.com/stretchr/testify from 1.8.2 to 1.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/stretchr/testify](https://github.com/stretchr/testify) from 1.8.2 to 1.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/stretchr/testify/releases">github.com/stretchr/testify's releases</a>.</em></p>
<blockquote>
<h2>v1.9.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix Go modules version by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1394">stretchr/testify#1394</a></li>
<li>Document that require is not safe to call in created goroutines by <a href="https://github.com/programmer04"><code>@​programmer04</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1392">stretchr/testify#1392</a></li>
<li>Remove myself from MAINTAINERS.md by <a href="https://github.com/mvdkleijn"><code>@​mvdkleijn</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1367">stretchr/testify#1367</a></li>
<li>Correct spelling/grammar by <a href="https://github.com/echarrod"><code>@​echarrod</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1389">stretchr/testify#1389</a></li>
<li>docs: Update URLs in README by <a href="https://github.com/davidjb"><code>@​davidjb</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1349">stretchr/testify#1349</a></li>
<li>Update mockery link to Github Pages in README by <a href="https://github.com/LandonTClipp"><code>@​LandonTClipp</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1346">stretchr/testify#1346</a></li>
<li>docs: Fix typos in tests and comments by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1410">stretchr/testify#1410</a></li>
<li>CI: tests from go1.17 by <a href="https://github.com/SuperQ"><code>@​SuperQ</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1409">stretchr/testify#1409</a></li>
<li>Fix adding ? when no values passed by <a href="https://github.com/lesichkovm"><code>@​lesichkovm</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1320">stretchr/testify#1320</a></li>
<li>codegen: use standard header for generated files by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1406">stretchr/testify#1406</a></li>
<li>mock: AssertExpectations log reason only on failure by <a href="https://github.com/hikyaru-suzuki"><code>@​hikyaru-suzuki</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1360">stretchr/testify#1360</a></li>
<li>assert: fix flaky TestNeverTrue by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1417">stretchr/testify#1417</a></li>
<li>README: fix typos &quot;set up&quot; vs &quot;setup&quot; by <a href="https://github.com/ossan-dev"><code>@​ossan-dev</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1428">stretchr/testify#1428</a></li>
<li>mock: move regexp compilation outside of <code>Called</code> by <a href="https://github.com/aud10slave"><code>@​aud10slave</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/631">stretchr/testify#631</a></li>
<li>assert: refactor internal func getLen() by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1445">stretchr/testify#1445</a></li>
<li>mock: deprecate type AnythingOfTypeArgument (<a href="https://redirect.github.com/stretchr/testify/issues/1434">#1434</a>) by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1441">stretchr/testify#1441</a></li>
<li>Remove no longer needed assert.canConvert by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1470">stretchr/testify#1470</a></li>
<li>assert: ObjectsAreEqual: use time.Equal for time.Time types by <a href="https://github.com/tscales"><code>@​tscales</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1464">stretchr/testify#1464</a></li>
<li>Bump actions/checkout from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1466">stretchr/testify#1466</a></li>
<li>Bump actions/setup-go from 3.2.0 to 4.1.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1451">stretchr/testify#1451</a></li>
<li>fix: make EventuallyWithT concurrency safe by <a href="https://github.com/czeslavo"><code>@​czeslavo</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1395">stretchr/testify#1395</a></li>
<li>assert: fix httpCode and HTTPBody occur panic when http.Handler read Body by <a href="https://github.com/hidu"><code>@​hidu</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1484">stretchr/testify#1484</a></li>
<li>assert.EqualExportedValues: fix handling of arrays by <a href="https://github.com/zrbecker"><code>@​zrbecker</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1473">stretchr/testify#1473</a></li>
<li>.github: use latest Go versions by <a href="https://github.com/kevinburkesegment"><code>@​kevinburkesegment</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1489">stretchr/testify#1489</a></li>
<li>assert: Deprecate EqualExportedValues by <a href="https://github.com/HaraldNordgren"><code>@​HaraldNordgren</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1488">stretchr/testify#1488</a></li>
<li>suite: refactor test assertions by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1474">stretchr/testify#1474</a></li>
<li>suite: fix SetupSubTest and TearDownSubTest execution order by <a href="https://github.com/linusbarth"><code>@​linusbarth</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1471">stretchr/testify#1471</a></li>
<li>docs: Fix deprecation comments for http package by <a href="https://github.com/alexandear"><code>@​alexandear</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1335">stretchr/testify#1335</a></li>
<li>Add map support doc comments to Subset and NotSubset by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1306">stretchr/testify#1306</a></li>
<li>TestErrorIs/TestNotErrorIs: check error message contents by <a href="https://github.com/craig65535"><code>@​craig65535</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1435">stretchr/testify#1435</a></li>
<li>suite: fix subtest names (fix <a href="https://redirect.github.com/stretchr/testify/issues/1501">#1501</a>) by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1504">stretchr/testify#1504</a></li>
<li>assert: improve unsafe.Pointer tests by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1505">stretchr/testify#1505</a></li>
<li>assert: simplify isNil implementation by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1506">stretchr/testify#1506</a></li>
<li>assert.InEpsilonSlice: fix expected/actual order and other improvements by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1483">stretchr/testify#1483</a></li>
<li>Fix dependency cycle with objx <a href="https://redirect.github.com/stretchr/testify/issues/1292">#1292</a> by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1453">stretchr/testify#1453</a></li>
<li>mock: refactor TestIsArgsEqual by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1444">stretchr/testify#1444</a></li>
<li>mock: optimize argument matching checks by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1416">stretchr/testify#1416</a></li>
<li>assert: fix TestEventuallyTimeout by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1412">stretchr/testify#1412</a></li>
<li>CI: add go 1.21 in GitHub Actions by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1450">stretchr/testify#1450</a></li>
<li>suite: fix recoverAndFailOnPanic to report test failure at the right location by <a href="https://github.com/dolmen"><code>@​dolmen</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1502">stretchr/testify#1502</a></li>
<li>Update maintainers by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1533">stretchr/testify#1533</a></li>
<li>assert: Fix EqualValues to handle overflow/underflow by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1531">stretchr/testify#1531</a></li>
<li>assert: better formatting for Len() error by <a href="https://github.com/kevinburkesegment"><code>@​kevinburkesegment</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1485">stretchr/testify#1485</a></li>
<li>Ensure AssertExpectations does not fail in skipped tests by <a href="https://github.com/ianrose14"><code>@​ianrose14</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1331">stretchr/testify#1331</a></li>
<li>suite: fix deadlock in suite.Require()/Assert() by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1535">stretchr/testify#1535</a></li>
<li>Revert &quot;assert: ObjectsAreEqual: use time.Equal for time.Time type&quot; by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1537">stretchr/testify#1537</a></li>
<li>[chore] Add issue templates by <a href="https://github.com/arjunmahishi"><code>@​arjunmahishi</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1538">stretchr/testify#1538</a></li>
<li>Update the build status badge by <a href="https://github.com/brackendawson"><code>@​brackendawson</code></a> in <a href="https://redirect.github.com/stretchr/testify/pull/1540">stretchr/testify#1540</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/stretchr/testify/commit/bb548d0473d4e1c9b7bbfd6602c7bf12f7a84dd2"><code>bb548d0</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1552">#1552</a> from stretchr/dependabot/go_modules/github.com/stret...</li>
<li><a href="https://github.com/stretchr/testify/commit/814075f391adffd2bf2b5110a74c51827ba132c4"><code>814075f</code></a> build(deps): bump github.com/stretchr/objx from 0.5.1 to 0.5.2</li>
<li><a href="https://github.com/stretchr/testify/commit/e0456122451b1839c8d58d32df6364e4d0f0a709"><code>e045612</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1339">#1339</a> from bogdandrutu/uintptr</li>
<li><a href="https://github.com/stretchr/testify/commit/5b6926d686d412518f50e888b9ae9b938355e011"><code>5b6926d</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1385">#1385</a> from hslatman/not-implements</li>
<li><a href="https://github.com/stretchr/testify/commit/9f97d67703eff02136d487e6c907e76fdea31a8b"><code>9f97d67</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1550">#1550</a> from stretchr/release-notes</li>
<li><a href="https://github.com/stretchr/testify/commit/bcb0d3fe49ff300fb78288cc144bc61a881f58ec"><code>bcb0d3f</code></a> Include the auto-release notes in releases</li>
<li><a href="https://github.com/stretchr/testify/commit/fb770f8238261aa22f8e0c56f18168ccb90f4a09"><code>fb770f8</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1247">#1247</a> from ccoVeille/typos</li>
<li><a href="https://github.com/stretchr/testify/commit/85d8bb6eea715dcbbb68f7c87b50e1956e20f892"><code>85d8bb6</code></a> fix typos in comments, tests and github templates</li>
<li><a href="https://github.com/stretchr/testify/commit/e2741fa4e9bf2fdfe3ed48d976a7eeebe76c5009"><code>e2741fa</code></a> Merge pull request <a href="https://redirect.github.com/stretchr/testify/issues/1548">#1548</a> from arjunmahishi/msgAndArgs</li>
<li><a href="https://github.com/stretchr/testify/commit/6e59f20c0d3883d2bdc589a9e48374ea30601851"><code>6e59f20</code></a> http_assertions: assert that the msgAndArgs actually works in tests</li>
<li>Additional commits viewable in <a href="https://github.com/stretchr/testify/compare/v1.8.2...v1.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/stretchr/testify&package-manager=go_modules&previous-version=1.8.2&new-version=1.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-04 04:44:55 +0000 UTC
    </div>
</div>

