---
layout: default
title: fabric-contract-api-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-contract-api-go
---

# fabric-contract-api-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-contract-api-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    Allow schema types with the same name from different packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the short type name was used as a schema key. This meant that types of the same name from different packages would overwrite each other in the map of schema type definitions, causing unexpected serialization errors. Now the fully qualified (package + type) name is used so that entries for types with the same name from different packages are unique.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 12:02:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.7.0 to 0.17.0 in /integrationtest/chaincode/transactionhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.7.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.7.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.7.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-contract-api-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 14:48:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    Bump protobufjs from 6.11.3 to 6.11.4 in /integrationtest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.11.3 to 6.11.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/protobufjs/protobuf.js/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.11.3&new-version=6.11.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-contract-api-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 14:48:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/115" class=".btn">#115</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.53.0 to 1.56.3 in /integrationtest/chaincode/transactionhooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.53.0 to 1.56.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.56.3</h2>
<h1>Security</h1>
<ul>
<li>
<p>server: prohibit more than MaxConcurrentStreams handlers from running at once (CVE-2023-44487)</p>
<p>In addition to this change, applications should ensure they do not leave running tasks behind related to the RPC before returning from method handlers, or should enforce appropriate limits on any such work.</p>
</li>
</ul>
<h2>Release 1.56.2</h2>
<ul>
<li>status: To fix a panic, <code>status.FromError</code> now returns an error with <code>codes.Unknown</code> when the error implements the <code>GRPCStatus()</code> method, and calling <code>GRPCStatus()</code> returns <code>nil</code>. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6374">#6374</a>)</li>
</ul>
<h2>Release 1.56.1</h2>
<ul>
<li>client: handle empty address lists correctly in addrConn.updateAddrs</li>
</ul>
<h2>Release 1.56.0</h2>
<h1>New Features</h1>
<ul>
<li>client: support channel idleness using <code>WithIdleTimeout</code> dial option (<a href="https://redirect.github.com/grpc/grpc-go/issues/6263">#6263</a>)
<ul>
<li>This feature is currently disabled by default, but will be enabled with a 30 minute default in the future.</li>
</ul>
</li>
<li>client: when using pickfirst, keep channel state in TRANSIENT_FAILURE until it becomes READY (<a href="https://github.com/grpc/proposal/blob/master/A62-pick-first.md">gRFC A62</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6306">#6306</a>)</li>
<li>xds: Add support for Custom LB Policies (<a href="https://github.com/grpc/proposal/blob/master/A52-xds-custom-lb-policies.md">gRFC A52</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6224">#6224</a>)</li>
<li>xds: support pick_first Custom LB policy (<a href="https://github.com/grpc/proposal/blob/master/A62-pick-first.md">gRFC A62</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6314">#6314</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6317">#6317</a>)</li>
<li>client: add support for pickfirst address shuffling (<a href="https://github.com/grpc/proposal/blob/master/A62-pick-first.md">gRFC A62</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6311">#6311</a>)</li>
<li>xds: Add support for String Matcher Header Matcher in RDS (<a href="https://redirect.github.com/grpc/grpc-go/issues/6313">#6313</a>)</li>
<li>xds/outlierdetection: Add Channelz Logger to Outlier Detection LB (<a href="https://redirect.github.com/grpc/grpc-go/issues/6145">#6145</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/s-matyukevich"><code>@​s-matyukevich</code></a></li>
</ul>
</li>
<li>xds: enable RLS in xDS by default (<a href="https://redirect.github.com/grpc/grpc-go/issues/6343">#6343</a>)</li>
<li>orca: add support for application_utilization field and missing range checks on several metrics setters</li>
<li>balancer/weightedroundrobin: add new LB policy for balancing between backends based on their load reports (<a href="https://github.com/grpc/proposal/blob/master/A58-client-side-weighted-round-robin-lb-policy.md">gRFC A58</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6241">#6241</a>)</li>
<li>authz: add conversion of json to RBAC Audit Logging config (<a href="https://redirect.github.com/grpc/grpc-go/issues/6192">#6192</a>)</li>
<li>authz: add support for stdout logger (<a href="https://redirect.github.com/grpc/grpc-go/issues/6230">#6230</a> and <a href="https://redirect.github.com/grpc/grpc-go/issues/6298">#6298</a>)</li>
<li>authz: support customizable audit functionality for authorization policy (<a href="https://redirect.github.com/grpc/grpc-go/issues/6192">#6192</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6230">#6230</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6298">#6298</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6158">#6158</a> <a href="https://redirect.github.com/grpc/grpc-go/issues/6304">#6304</a> and <a href="https://redirect.github.com/grpc/grpc-go/issues/6225">#6225</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>orca: fix a race at startup of out-of-band metric subscriptions that would cause the report interval to request 0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6245">#6245</a>)</li>
<li>xds/xdsresource: Fix Outlier Detection Config Handling and correctly set xDS Defaults (<a href="https://redirect.github.com/grpc/grpc-go/issues/6361">#6361</a>)</li>
<li>xds/outlierdetection: Fix Outlier Detection Config Handling by setting defaults in ParseConfig() (<a href="https://redirect.github.com/grpc/grpc-go/issues/6361">#6361</a>)</li>
</ul>
<h1>API Changes</h1>
<ul>
<li>orca: allow a ServerMetricsProvider to be passed to the ORCA service and ServerOption (<a href="https://redirect.github.com/grpc/grpc-go/issues/6223">#6223</a>)</li>
</ul>
<h2>Release 1.55.1</h2>
<ul>
<li>status: To fix a panic, <code>status.FromError</code> now returns an error with <code>codes.Unknown</code> when the error implements the <code>GRPCStatus()</code> method, and calling <code>GRPCStatus()</code> returns <code>nil</code>. (<a href="https://redirect.github.com/grpc/grpc-go/issues/6374">#6374</a>)</li>
</ul>
<h2>Release 1.55.0</h2>
<h1>Behavior Changes</h1>
<ul>
<li>xds: enable federation support by default (<a href="https://redirect.github.com/grpc/grpc-go/issues/6151">#6151</a>)</li>
<li>status: <code>status.Code</code> and <code>status.FromError</code> handle wrapped errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/6031">#6031</a> and <a href="https://redirect.github.com/grpc/grpc-go/issues/6150">#6150</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/1055b481ed2204a29d233286b9b50c42b63f8825"><code>1055b48</code></a> Update version.go to 1.56.3 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6713">#6713</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/5efd7bd73e11fea58d1c7f1c110902e78a286299"><code>5efd7bd</code></a> server: prohibit more than MaxConcurrentStreams handlers from running at once...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bd1f038e7234580c2694e433bec5cd97e7b7f662"><code>bd1f038</code></a> Upgrade version.go to 1.56.3-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6434">#6434</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/faab8736bf73291f92b867d5dae31c927d53d508"><code>faab873</code></a> Update version.go to v1.56.2 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6432">#6432</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/6b0b291d79831b1c8caafceec268b82c92253f96"><code>6b0b291</code></a> status: fix panic when servers return a wrapped error with status OK (<a href="https://redirect.github.com/grpc/grpc-go/issues/6374">#6374</a>) ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/ed56401aa514462d5371713b8ec5c889da33953c"><code>ed56401</code></a> [PSM interop] Don't fail target if sub-target already failed (<a href="https://redirect.github.com/grpc/grpc-go/issues/6390">#6390</a>) (<a href="https://redirect.github.com/grpc/grpc-go/issues/6405">#6405</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/cd6a794f0bdcf9a216e8f4d3c5717faf96d9fd78"><code>cd6a794</code></a> Update version.go to v1.56.2-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6387">#6387</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/5b67e5ea449ef0686a0c0b6de48cd4cb63e3db2a"><code>5b67e5e</code></a> Update version.go to v1.56.1 (<a href="https://redirect.github.com/grpc/grpc-go/issues/6386">#6386</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/d0f5150384a87f9fcac488a9c18727a55b7354c1"><code>d0f5150</code></a> client: handle empty address lists correctly in addrConn.updateAddrs (<a href="https://redirect.github.com/grpc/grpc-go/issues/6354">#6354</a>) ...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/997c1ea101cc5d496d2b148388f1df49632a9171"><code>997c1ea</code></a> Change version to 1.56.1-dev (<a href="https://redirect.github.com/grpc/grpc-go/issues/6345">#6345</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.53.0...v1.56.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.53.0&new-version=1.56.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-contract-api-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 14:48:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    Bump get-func-name from 2.0.0 to 2.0.2 in /integrationtest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [get-func-name](https://github.com/chaijs/get-func-name) from 2.0.0 to 2.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/chaijs/get-func-name/releases">get-func-name's releases</a>.</em></p>
<blockquote>
<h2>v2.0.2</h2>
<h2>What's Changed</h2>
<p>Revert previous changes that shipped this as an ES module.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/chaijs/get-func-name/commits/v2.0.2">https://github.com/chaijs/get-func-name/commits/v2.0.2</a></p>
<h2>v2.0.1</h2>
<h2>What's Changed</h2>
<p>Fix <a href="https://github.com/chaijs/get-func-name/security/advisories/GHSA-4q6p-r6v2-jvc5">https://github.com/chaijs/get-func-name/security/advisories/GHSA-4q6p-r6v2-jvc5</a></p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/chaijs/get-func-name/commits/v2.0.1">https://github.com/chaijs/get-func-name/commits/v2.0.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/chaijs/get-func-name/commits/v2.0.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~keithamus">keithamus</a>, a new releaser for get-func-name since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=get-func-name&package-manager=npm_and_yarn&previous-version=2.0.0&new-version=2.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-contract-api-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 14:48:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/112" class=".btn">#112</a>
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
        Created At 2023-11-06 15:19:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-contract-api-go/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Bump github.com/cucumber/godog from 0.12.6 to 0.13.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/cucumber/godog](https://github.com/cucumber/godog) from 0.12.6 to 0.13.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/cucumber/godog/releases">github.com/cucumber/godog's releases</a>.</em></p>
<blockquote>
<h2>v0.13.0</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(*): BREAKING CHANGE, use new repos for cucumber and messages by <a href="https://github.com/otrava7"><code>@​otrava7</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/515">cucumber/godog#515</a></li>
<li>Configure Renovate by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/512">cucumber/godog#512</a></li>
<li>fix(deps): update module github.com/cucumber/godog to v0.12.6 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/520">cucumber/godog#520</a></li>
<li>chore(deps): update codecov/codecov-action action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/530">cucumber/godog#530</a></li>
<li>chore(deps): update actions/checkout action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/528">cucumber/godog#528</a></li>
<li>chore(deps): update actions/setup-go action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/529">cucumber/godog#529</a></li>
<li>chore(deps): update actions/cache action to v3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/527">cucumber/godog#527</a></li>
<li>fix(deps): update module github.com/cucumber/gherkin/go/v26 to v26.0.3 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/519">cucumber/godog#519</a></li>
<li>fix(deps): update module github.com/data-dog/go-txdb to v0.1.5 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/522">cucumber/godog#522</a></li>
<li>fix(deps): update module github.com/go-sql-driver/mysql to v1.7.0 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/524">cucumber/godog#524</a></li>
<li>fix(deps): update module github.com/hashicorp/go-memdb to v1.3.4 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/523">cucumber/godog#523</a></li>
<li>fix(deps): update module github.com/spf13/cobra to v1.6.1 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/526">cucumber/godog#526</a></li>
<li>fix(deps): update module github.com/smartystreets/goconvey to v1.7.2 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/525">cucumber/godog#525</a></li>
<li>Setup Renovate with default Configs by <a href="https://github.com/mpkorstanje"><code>@​mpkorstanje</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/531">cucumber/godog#531</a></li>
<li>Implement unambiguous keywords by <a href="https://github.com/otrava7"><code>@​otrava7</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/509">cucumber/godog#509</a></li>
<li>docs(*): correct example by <a href="https://github.com/otrava7"><code>@​otrava7</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/538">cucumber/godog#538</a></li>
<li>fix(deps): update module github.com/data-dog/go-txdb to v0.1.6 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/540">cucumber/godog#540</a></li>
<li>fix(deps): update module github.com/stretchr/testify to v1.8.2 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/541">cucumber/godog#541</a></li>
<li>chore(deps): update actions/setup-go action to v4 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/546">cucumber/godog#546</a></li>
<li>docs: prefer go test to use of godog cli in README by <a href="https://github.com/danielhelfand"><code>@​danielhelfand</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/548">cucumber/godog#548</a></li>
<li>Use <code>fs.FS</code> abstraction for filesystem by <a href="https://github.com/tigh-latte"><code>@​tigh-latte</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/550">cucumber/godog#550</a></li>
<li>Result of testing.T respect strict option by <a href="https://github.com/eiel"><code>@​eiel</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/539">cucumber/godog#539</a></li>
<li>Update CI for go1.20 by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/552">cucumber/godog#552</a></li>
<li>fix(deps): update module github.com/cucumber/gherkin/go/v26 to v26.1.0 by <a href="https://github.com/renovate"><code>@​renovate</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/549">cucumber/godog#549</a></li>
<li>cancel context for each scenario by <a href="https://github.com/draganm"><code>@​draganm</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/514">cucumber/godog#514</a></li>
<li>Use staticcheck GitHub Action by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/563">cucumber/godog#563</a></li>
<li>refactor: test_context.go by <a href="https://github.com/longyue0521"><code>@​longyue0521</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/564">cucumber/godog#564</a></li>
<li>Improve hooks invocation flow by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/568">cucumber/godog#568</a></li>
<li>fix(examples): update api example by <a href="https://github.com/forward32"><code>@​forward32</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/532">cucumber/godog#532</a></li>
<li>Improve example with concurrency support by <a href="https://github.com/vearutop"><code>@​vearutop</code></a> in <a href="https://redirect.github.com/cucumber/godog/pull/573">cucumber/godog#573</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/otrava7"><code>@​otrava7</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/515">cucumber/godog#515</a></li>
<li><a href="https://github.com/renovate"><code>@​renovate</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/512">cucumber/godog#512</a></li>
<li><a href="https://github.com/mpkorstanje"><code>@​mpkorstanje</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/531">cucumber/godog#531</a></li>
<li><a href="https://github.com/danielhelfand"><code>@​danielhelfand</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/548">cucumber/godog#548</a></li>
<li><a href="https://github.com/tigh-latte"><code>@​tigh-latte</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/550">cucumber/godog#550</a></li>
<li><a href="https://github.com/eiel"><code>@​eiel</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/539">cucumber/godog#539</a></li>
<li><a href="https://github.com/draganm"><code>@​draganm</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/514">cucumber/godog#514</a></li>
<li><a href="https://github.com/longyue0521"><code>@​longyue0521</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/564">cucumber/godog#564</a></li>
<li><a href="https://github.com/forward32"><code>@​forward32</code></a> made their first contribution in <a href="https://redirect.github.com/cucumber/godog/pull/532">cucumber/godog#532</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/cucumber/godog/compare/v0.12.6...v0.13.0">https://github.com/cucumber/godog/compare/v0.12.6...v0.13.0</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/cucumber/godog/blob/main/CHANGELOG.md">github.com/cucumber/godog's changelog</a>.</em></p>
<blockquote>
<h2>[v0.13.0]</h2>
<h3>Added</h3>
<ul>
<li>Support for reading feature files from an <code>fs.FS</code> (<a href="https://redirect.github.com/cucumber/godog/pull/550">550</a> - <a href="https://github.com/tigh-latte">tigh-latte</a>)</li>
<li>Added keyword functions. (<a href="https://redirect.github.com/cucumber/godog/pull/509">509</a> - <a href="https://github.com/otrava7">otrava7</a>)</li>
<li>Prefer go test to use of godog cli in README (<a href="https://redirect.github.com/cucumber/godog/pull/548">548</a> - <a href="https://github.com/danielhelfand">danielhelfand</a>)</li>
<li>Use <code>fs.FS</code> abstraction for filesystem (<a href="https://redirect.github.com/cucumber/godog/pull/550">550</a> - <a href="https://github.com/tigh-latte">tigh-latte</a>)</li>
<li>Cancel context for each scenario (<a href="https://redirect.github.com/cucumber/godog/pull/514">514</a> - <a href="https://github.com/draganm">draganm</a>)</li>
</ul>
<h3>Fixed</h3>
<ul>
<li>Improve hooks invocation flow (<a href="https://redirect.github.com/cucumber/godog/pull/568">568</a> - <a href="https://github.com/vearutop">vearutop</a>)</li>
<li>Result of testing.T respect strict option (<a href="https://redirect.github.com/cucumber/godog/pull/539">539</a> - <a href="https://github.com/eiel">eiel</a>)</li>
</ul>
<h3>Changed</h3>
<ul>
<li>BREAKING CHANGE, upgraded cucumber and messages dependencies = (<a href="https://redirect.github.com/cucumber/godog/pull/515">515</a> - <a href="https://github.com/otrava7">otrava7</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/cucumber/godog/commit/6b96d47e70b95ff62bb240aff3e588569b7d19b2"><code>6b96d47</code></a> Prepare CHANGELOG.md for new release</li>
<li><a href="https://github.com/cucumber/godog/commit/d3aec7142e95ad5a0c9ec849e72d3accef089040"><code>d3aec71</code></a> Improve example with concurrency support (<a href="https://redirect.github.com/cucumber/godog/issues/573">#573</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/75d5cab90d0443b1eff2903a4fbfbdb6e594a139"><code>75d5cab</code></a> fix(examples): update api example (<a href="https://redirect.github.com/cucumber/godog/issues/532">#532</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/3e0f9026f3ddb697b9e4e82b0e770fbbe0e966b7"><code>3e0f902</code></a> Improve hooks invocation flow (<a href="https://redirect.github.com/cucumber/godog/issues/568">#568</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/51d164ff5789b10ad013c6db4099f4499f1a31a0"><code>51d164f</code></a> Print verbose error to enable traces</li>
<li><a href="https://github.com/cucumber/godog/commit/72db47c51993eb6d29378cbda01e24fae4156c7f"><code>72db47c</code></a> refactor: test_context.go (<a href="https://redirect.github.com/cucumber/godog/issues/564">#564</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/ea50e4bdfcd911252e39f303b9327197079be1e4"><code>ea50e4b</code></a> Use staticcheck GitHub Action (<a href="https://redirect.github.com/cucumber/godog/issues/563">#563</a>)</li>
<li><a href="https://github.com/cucumber/godog/commit/7f75c5d4ee9cd2e9d86b7ff62ebf38b9172d2c88"><code>7f75c5d</code></a> Remove redundant return</li>
<li><a href="https://github.com/cucumber/godog/commit/35820ff9fee90f20afdc1c20a7e5e7c4d6c59ebb"><code>35820ff</code></a> Reduce deps, fix CI for go1.16, format imports</li>
<li><a href="https://github.com/cucumber/godog/commit/3eae6c04373960d397e20e1d24cc8ee4210af72e"><code>3eae6c0</code></a> Update dependencies</li>
<li>Additional commits viewable in <a href="https://github.com/cucumber/godog/compare/v0.12.6...v0.13.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/cucumber/godog&package-manager=go_modules&previous-version=0.12.6&new-version=0.13.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-06 15:19:01 +0000 UTC
    </div>
</div>

