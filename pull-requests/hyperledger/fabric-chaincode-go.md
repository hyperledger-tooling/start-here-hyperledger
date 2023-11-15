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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.54.0 to 1.59.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.54.0 to 1.59.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.58.3</h2>
<h1>Security</h1>
<ul>
<li>
<p>server: prohibit more than MaxConcurrentStreams handlers from running at once (CVE-2023-44487)</p>
<p>In addition to this change, applications should ensure they do not leave running tasks behind related to the RPC before returning from method handlers, or should enforce appropriate limits on any such work.</p>
</li>
</ul>
<h2>Release 1.58.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>
<p>balancer/weighted_round_robin: fix ticker leak on update</p>
<p>A new ticker is created every time there is an update of addresses or configuration, but was not properly stopped.  This change stops the ticker when it is no longer needed.</p>
</li>
</ul>
<h2>Release 1.58.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpc: fix a bug that was decrementing active RPC count too early for streaming RPCs; leading to channel moving to IDLE even though it had open streams</li>
<li>grpc: fix a bug where transports were not being closed upon channel entering IDLE</li>
</ul>
<h2>Release 1.58.0</h2>
<h1>API Changes</h1>
<p>See <a href="https://redirect.github.com/grpc/grpc-go/issues/6472">#6472</a> for details about these changes.</p>
<ul>
<li>balancer: add <code>StateListener</code> to <code>NewSubConnOptions</code> for <code>SubConn</code> state updates and deprecate <code>Balancer.UpdateSubConnState</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6481">#6481</a>)
<ul>
<li><code>UpdateSubConnState</code> will be deleted in the future.</li>
</ul>
</li>
<li>balancer: add <code>SubConn.Shutdown</code> and deprecate <code>Balancer.RemoveSubConn</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6493">#6493</a>)
<ul>
<li><code>RemoveSubConn</code> will be deleted in the future.</li>
</ul>
</li>
<li>resolver: remove deprecated <code>AddressType</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6451">#6451</a>)
<ul>
<li>This was previously used as a signal to enable the &quot;grpclb&quot; load balancing policy, and to pass LB addresses to the policy.  Instead, <code>balancer/grpclb/state.Set()</code> should be used to add these addresses to the name resolver's output.  The built-in &quot;dns&quot; name resolver already does this.</li>
</ul>
</li>
<li>resolver: add new field <code>Endpoints</code> to <code>State</code> and deprecate <code>Addresses</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6471">#6471</a>)
<ul>
<li><code>Addresses</code> will be deleted in the future.</li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>balancer/leastrequest: Add experimental support for least request LB policy and least request configured as a custom xDS policy (<a href="https://redirect.github.com/grpc/grpc-go/issues/6510">#6510</a>, <a href="https://redirect.github.com/grpc/grpc-go/issues/6517">#6517</a>)
<ul>
<li>Set <code>GRPC_EXPERIMENTAL_ENABLE_LEAST_REQUEST=true</code> to enable</li>
</ul>
</li>
<li>stats: Add an RPC event for blocking caused by the LB policy's picker (<a href="https://redirect.github.com/grpc/grpc-go/issues/6422">#6422</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>clusterresolver: fix deadlock when dns resolver responds inline with update or error at build time (<a href="https://redirect.github.com/grpc/grpc-go/issues/6563">#6563</a>)</li>
<li>grpc: fix a bug where the channel could erroneously report <code>TRANSIENT_FAILURE</code> when actually moving to <code>IDLE</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/6497">#6497</a>)</li>
<li>balancergroup: do not cache closed sub-balancers by default; affects <code>rls</code>, <code>weightedtarget</code> and <code>clustermanager</code> LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/6523">#6523</a>)</li>
<li>client: fix a bug that prevented detection of RPC status in trailers-only RPC responses when using <code>ClientStream.Header()</code>, and prevented retry of the RPC (<a href="https://redirect.github.com/grpc/grpc-go/issues/6557">#6557</a>)</li>
</ul>
<h1>Performance Improvements</h1>
<ul>
<li>client &amp; server: Add experimental <code>[With]SharedWriteBuffer</code> to improve performance by reducing allocations when sending RPC messages. (Disabled by default.) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6309">#6309</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/s-matyukevich"><code>@​s-matyukevich</code></a></li>
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
<li><a href="https://github.com/grpc/grpc-go/commit/7765221f4bf6104973db7946d56936cf838cad46"><code>7765221</code></a> Change version to 1.59.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6695">#6695</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e88f12e0517d465cb892ef58e1debf10b4e5607f"><code>e88f12e</code></a> server: prohibit more than MaxConcurrentStreams handlers from running at once...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/be7919c3dc3c26f54489c778af7bbfea608ad9bc"><code>be7919c</code></a> transport: Pass Header metadata to tap handle. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6652">#6652</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e3f1514cdb8fcbcacc30b53473042dbb40a54791"><code>e3f1514</code></a> Reapply &quot;status: fix/improve status handling (<a href="https://redirect.github.com/grpc/grpc-go/issues/6662">#6662</a>)&quot; (<a href="https://redirect.github.com/grpc/grpc-go/issues/6673">#6673</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6688">#6688</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/696faa982cdc0914929a64848a8ff3bf7a924166"><code>696faa9</code></a> client: add a test for NewSubConn / StateListener / cc.Close racing (<a href="https://redirect.github.com/grpc/grpc-go/issues/6678">#6678</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/318c717a659ec55a2f92e1c84313153dd278bf55"><code>318c717</code></a> readme: fix badges (<a href="https://redirect.github.com/grpc/grpc-go/issues/6687">#6687</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/39972fdd744873a2b829ab98962ab0e85800d591"><code>39972fd</code></a> github: add code coverage with codecov.io (<a href="https://redirect.github.com/grpc/grpc-go/issues/6676">#6676</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/93dbc059f561340a14aeb96ea2925b9a669c5673"><code>93dbc05</code></a> xds: move virtual host matcher test to the xdsresource package (<a href="https://redirect.github.com/grpc/grpc-go/issues/6680">#6680</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2c00469782f1dd8c7456dcc7238a957781246e84"><code>2c00469</code></a> github: update actions/setup-go and actions/checkout (<a href="https://redirect.github.com/grpc/grpc-go/issues/6675">#6675</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/1f73ed5fcf75b3e464c83ab17fc73144e2161620"><code>1f73ed5</code></a> Replace the gRFC pull request with the permanent link. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6674">#6674</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.54.0...v1.59.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.54.0&new-version=1.59.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-09 04:23:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    Bump github.com/stretchr/testify from 1.8.2 to 1.8.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/stretchr/testify](https://github.com/stretchr/testify) from 1.8.2 to 1.8.4.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/stretchr/testify/commit/f97607b89807936ac4ff96748d766cf4b9711f78"><code>f97607b</code></a> Create GitHub release when new release tag is pushed (<a href="https://redirect.github.com/stretchr/testify/issues/1354">#1354</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/4c93d8f201cb46ed50de949ee65804f944b570f8"><code>4c93d8f</code></a> EqualExportedValues: Handle nested pointer, slice and map fields (<a href="https://redirect.github.com/stretchr/testify/issues/1379">#1379</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/4b2f4d2bcff3848b6a4e63d462da6ce3c21e9c78"><code>4b2f4d2</code></a> add EventuallyWithT assertion (<a href="https://redirect.github.com/stretchr/testify/issues/1264">#1264</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/b3106d772c7aa439743e1a3f4de81149e323cf70"><code>b3106d7</code></a> allow testing for functional options (<a href="https://redirect.github.com/stretchr/testify/issues/1023">#1023</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/437071b948cd89bdbaaf43a41f19fbe1a0945f6f"><code>437071b</code></a> assert: fix error message formatting for NotContains (<a href="https://redirect.github.com/stretchr/testify/issues/1362">#1362</a>)</li>
<li><a href="https://github.com/stretchr/testify/commit/c5fc9d6b6b21ea89be8480c0dc35e2977ab988f6"><code>c5fc9d6</code></a> Compare public elements of struct (<a href="https://redirect.github.com/stretchr/testify/issues/1309">#1309</a>)</li>
<li>See full diff in <a href="https://github.com/stretchr/testify/compare/v1.8.2...v1.8.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/stretchr/testify&package-manager=go_modules&previous-version=1.8.2&new-version=1.8.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-09 04:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-go/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    Bump github.com/hyperledger/fabric-protos-go from 0.3.0 to 0.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/hyperledger/fabric-protos-go](https://github.com/hyperledger/fabric-protos-go) from 0.3.0 to 0.3.1.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/212400245d309cf319fd0734ac18d60783d3a746"><code>2124002</code></a> Extend lifecycle protos to checkcommitreadiness to provide discrepancy details</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/b03edb47a905a20294e668e937d2035659852564"><code>b03edb4</code></a> system channel cleanup - make HeaderType_ORDERER_TRANSACTION deprecated (<a href="https://redirect.github.com/hyperledger/fabric-protos-go/issues/184">#184</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/8f302041c2e296480a3755906f72f5aab9bcc3ba"><code>8f30204</code></a> Bump Go to 1.19 (<a href="https://redirect.github.com/hyperledger/fabric-protos-go/issues/178">#178</a>)</li>
<li><a href="https://github.com/hyperledger/fabric-protos-go/commit/8b7f1c52afc671f1e64c3c18bf192078facaace2"><code>8b7f1c5</code></a> Update Go bindings build</li>
<li>See full diff in <a href="https://github.com/hyperledger/fabric-protos-go/compare/v0.3.0...v0.3.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/hyperledger/fabric-protos-go&package-manager=go_modules&previous-version=0.3.0&new-version=0.3.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-09 04:22:48 +0000 UTC
    </div>
</div>

