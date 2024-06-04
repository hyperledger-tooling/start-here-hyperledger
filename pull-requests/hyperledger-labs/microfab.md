---
layout: default
title: microfab
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/microfab
---

# microfab <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/microfab){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Enable TLS for Integration Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 20:36:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.52.0 to 1.56.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.52.0 to 1.56.3.
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
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.52.0...v1.56.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.52.0&new-version=1.56.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/microfab/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 19:30:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 23.0.0+incompatible to 24.0.9+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 23.0.0+incompatible to 24.0.9+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v24.0.9</h2>
<h2>24.0.9</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A24.0.9">docker/cli, 24.0.9 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A24.0.9">moby/moby, 24.0.9 milestone</a></li>
</ul>
<h2>Security</h2>
<p>This release contains security fixes for the following CVEs affecting Docker Engine and its components.</p>
<table>
<thead>
<tr>
<th>CVE</th>
<th>Component</th>
<th>Fix version</th>
<th>Severity</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://scout.docker.com/v/CVE-2024-21626">CVE-2024-21626</a></td>
<td>runc</td>
<td>1.1.12</td>
<td>High, CVSS 8.6</td>
</tr>
<tr>
<td><a href="https://scout.docker.com/v/CVE-2024-24557">CVE-2024-24557</a></td>
<td>Docker Engine</td>
<td>24.0.9</td>
<td>Medium, CVSS 6.9</td>
</tr>
</tbody>
</table>
<blockquote>
<p><strong>Important</strong> ⚠️</p>
<p>Note that this release of Docker Engine doesn't include fixes for the following known vulnerabilities in BuildKit:</p>
<ul>
<li><a href="https://scout.docker.com/v/CVE-2024-23651">CVE-2024-23651</a></li>
<li><a href="https://scout.docker.com/v/CVE-2024-23652">CVE-2024-23652</a></li>
<li><a href="https://scout.docker.com/v/CVE-2024-23653">CVE-2024-23653</a></li>
<li><a href="https://scout.docker.com/v/CVE-2024-23650">CVE-2024-23650</a></li>
</ul>
<p>To address these vulnerabilities, upgrade to <a href="https://github.com/docker/docker/blob/HEAD/25.0.md#2502">Docker Engine v25.0.2</a>.</p>
</blockquote>
<p>For more information about the security issues addressed in this release, and the unaddressed vulnerabilities in BuildKit, refer to the
<a href="https://www.docker.com/blog/docker-security-advisory-multiple-vulnerabilities-in-runc-buildkit-and-moby/">blog post</a>. For details about each vulnerability, see the relevant security advisory:</p>
<ul>
<li><a href="https://github.com/opencontainers/runc/security/advisories/GHSA-xr7r-f8xq-vfvv">CVE-2024-21626</a></li>
<li><a href="https://github.com/moby/moby/security/advisories/GHSA-xw73-rw38-6vjc">CVE-2024-24557</a></li>
</ul>
<h3>Packaging updates</h3>
<ul>
<li>Upgrade runc to <a href="https://github.com/opencontainers/runc/releases/tag/v1.1.12">v1.1.12</a>. <a href="https://redirect.github.com/moby/moby/pull/47269">moby/moby#47269</a></li>
<li>Upgrade containerd to <a href="https://github.com/containerd/containerd/releases/tag/v1.7.13">v1.7.13</a> (static binaries only). <a href="https://redirect.github.com/moby/moby/pull/47280">moby/moby#47280</a></li>
</ul>
<h2>v24.0.8</h2>
<h2>24.0.8</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A24.0.8">docker/cli, 24.0.8 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A24.0.8">moby/moby, 24.0.8 milestone</a></li>
</ul>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Live restore: Containers with auto remove (<code>docker run --rm</code>) are no longer forcibly removed on engine restart. <a href="https://redirect.github.com/moby/moby/pull/46869">moby/moby#46857</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/fca702de7f71362c8d103073c7e4a1d0a467fadd"><code>fca702d</code></a> Merge pull request from GHSA-xw73-rw38-6vjc</li>
<li><a href="https://github.com/moby/moby/commit/f78a7726d747847e443a5a5a4b4ad8ab31d87d78"><code>f78a772</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47281">#47281</a> from thaJeztah/24.0_backport_bump_containerd_binary...</li>
<li><a href="https://github.com/moby/moby/commit/61afffeeb3d4264db7a697ca8bd3d25824bee182"><code>61afffe</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47270">#47270</a> from thaJeztah/24.0_backport_bump_runc_binary_1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/b38e74c4e095d584e21576e9cc43a355446e5b71"><code>b38e74c</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47276">#47276</a> from thaJeztah/24.0_backport_bump_runc_1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/dac56638adccd215bae6cc23146f29e4697e1e98"><code>dac5663</code></a> update containerd binary to v1.7.13</li>
<li><a href="https://github.com/moby/moby/commit/20e1af361628a31afd1af58d25cd6ea4e495669f"><code>20e1af3</code></a> vendor: github.com/opencontainers/runc v1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/858919d39968c687de3afb0a0a3a212d60ef2a99"><code>858919d</code></a> update runc binary to v1.1.12</li>
<li><a href="https://github.com/moby/moby/commit/141ad39e38a9a44b7487933d74815863c2c588e6"><code>141ad39</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47266">#47266</a> from vvoland/ci-fix-makeps1-templatefail-24</li>
<li><a href="https://github.com/moby/moby/commit/db968c672bcd6eeed09a0ad35cac843a5ffe7e48"><code>db968c6</code></a> hack/make.ps1: Fix go list pattern</li>
<li><a href="https://github.com/moby/moby/commit/61c51fbb5aeb648eb5f97704b8c75be3ccf1c9a0"><code>61c51fb</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47221">#47221</a> from vvoland/pkg-pools-close-noop-24</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v23.0.0...v24.0.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=23.0.0+incompatible&new-version=24.0.9+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/microfab/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 19:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.4.0 to 0.23.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.4.0 to 0.23.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/c48da131589f122489348be5dfbcb6457640046f"><code>c48da13</code></a> http2: fix TestServerContinuationFlood flakes</li>
<li><a href="https://github.com/golang/net/commit/762b58d1cf6e0779780decad89c6c1523386638d"><code>762b58d</code></a> http2: fix tipos in comment</li>
<li><a href="https://github.com/golang/net/commit/ba872109ef2dc8f1da778651bd1fd3792d0e4587"><code>ba87210</code></a> http2: close connections when receiving too many headers</li>
<li><a href="https://github.com/golang/net/commit/ebc8168ac8ac742194df729305175940790c55a2"><code>ebc8168</code></a> all: fix some typos</li>
<li><a href="https://github.com/golang/net/commit/3678185f8a652e52864c44049a9ea96b7bcc066a"><code>3678185</code></a> http2: make TestCanonicalHeaderCacheGrowth faster</li>
<li><a href="https://github.com/golang/net/commit/448c44f9287b6745f958d74aa2a17ec7761c2f13"><code>448c44f</code></a> http2: remove clientTester</li>
<li><a href="https://github.com/golang/net/commit/c7877ac4213b2f859831366f5a35b353e0dc9f66"><code>c7877ac</code></a> http2: convert the remaining clientTester tests to testClientConn</li>
<li><a href="https://github.com/golang/net/commit/d8870b0bf2f2426fc8d19a9332f652da5c25418f"><code>d8870b0</code></a> http2: use synthetic time in TestIdleConnTimeout</li>
<li><a href="https://github.com/golang/net/commit/d73acffdc9493532acb85777105bb4a351eea702"><code>d73acff</code></a> http2: only set up deadline when Server.IdleTimeout is positive</li>
<li><a href="https://github.com/golang/net/commit/89f602b7bbf237abe0467031a18b42fc742ced08"><code>89f602b</code></a> http2: validate client/outgoing trailers</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.4.0...v0.23.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.4.0&new-version=0.23.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/microfab/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 19:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/protobuf from 1.28.1 to 1.33.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps google.golang.org/protobuf from 1.28.1 to 1.33.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/protobuf&package-manager=go_modules&previous-version=1.28.1&new-version=1.33.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/microfab/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 19:29:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/163" class=".btn">#163</a>
            </td>
            <td>
                <b>
                    Update pr.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update Node to Node20
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 19:14:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/microfab/pull/162" class=".btn">#162</a>
            </td>
            <td>
                <b>
                    Update docker image dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    Upgrade to golang 1.22.3
    Upgrade to Node 20.14.0
    Upgrade Fabric CA to 1.5.11
    Upgrade maven to 3.9.7
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 20:33:50 +0000 UTC
    </div>
</div>

