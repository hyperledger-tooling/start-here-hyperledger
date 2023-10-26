---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4495" class=".btn">#4495</a>
            </td>
            <td>
                <b>
                    fix : updated broken link in README file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Documentation update

#### Description

Updated the broken link of Hyperledge community to new link


<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->
This resolves #4494 

<!---
#### Release Note
-->



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-26 04:53:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4493" class=".btn">#4493</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.53.0 to 1.56.3
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 22:30:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4492" class=".btn">#4492</a>
            </td>
            <td>
                <b>
                    Use append to concatenate bytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I09e552881dab2a02a0b2b40f67d9f597975d90b4

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

In golang, append() can be used to append new elements to a slice.

The patchset simplify the code of method `ConcatenateBytes`.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 21:31:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4491" class=".btn">#4491</a>
            </td>
            <td>
                <b>
                    Simplify code by using direct return
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset simplifies the code by using direct return.

Change-Id: I3a9db0173fa0ae08adf53f3edb2d6e0a3a3e8678

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The method ExtractRemoteAddress uses two types of return:

1. direct return of "";
2. return the variable of remoteAddress

The patchset simplify the code by using direct return.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 21:17:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4490" class=".btn">#4490</a>
            </td>
            <td>
                <b>
                    Verify transactions in a block are well formed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Verify that transactions in blocks appear exactly as their marshaled form after unmarshaling. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 19:44:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4489" class=".btn">#4489</a>
            </td>
            <td>
                <b>
                    Update docs on checkcommitreadiness with inspect flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

This patch updates documents on `checkcommitreadiness` with `inspect` flag.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->
Resolve #4428

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 23:58:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4488" class=".btn">#4488</a>
            </td>
            <td>
                <b>
                    Removing nwo.DeployChaincodeLegacy()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit removes the DeployChaincodeLegacy function from the integration tests suite to address #3983 as part of eliminating the legacy chaincode lifecycle. Due to the changes in size, the work will be split into several PRs. This is the first one in a row.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-22 13:38:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4487" class=".btn">#4487</a>
            </td>
            <td>
                <b>
                    change workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                because of runner fabric-ubuntu, my fork stopped passing checks, tests and integration tests
<img width="783" alt="Снимок экрана 2023-10-21 в 23 41 55" src="https://github.com/hyperledger/fabric/assets/7284783/d423d6df-4847-40a6-90c3-670904dde4a0">


here is my solution, if anyone has a better one, you are welcome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-21 20:14:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4486" class=".btn">#4486</a>
            </td>
            <td>
                <b>
                    Verify hash chain in BFT
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
        Created At 2023-10-19 13:28:11 +0000 UTC
    </div>
</div>

