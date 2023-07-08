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
                PR <a href="https://github.com/hyperledger/fabric/pull/4309" class=".btn">#4309</a>
            </td>
            <td>
                <b>
                    add change and add unit tests
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

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

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
        Created At 2023-07-07 13:24:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4308" class=".btn">#4308</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.47.0 to 1.53.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [google.golang.org/grpc](https://github.com/grpc/grpc-go) from 1.47.0 to 1.53.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-go/releases">google.golang.org/grpc's releases</a>.</em></p>
<blockquote>
<h2>Release 1.53.0</h2>
<h1>API Changes</h1>
<ul>
<li>balancer: support injection of per-call metadata from LB policies (<a href="https://redirect.github.com/grpc/grpc-go/issues/5853">#5853</a>)</li>
<li>resolver: remove deprecated field <code>resolver.Target.Endpoint</code> and replace with <code>resolver.Target.Endpoint()</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/kylejb"><code>@​kylejb</code></a></li>
</ul>
</li>
</ul>
<h1>New Features</h1>
<ul>
<li>xds/ringhash: introduce <code>GRPC_RING_HASH_CAP</code> environment variable to override the maximum ring size. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5884">#5884</a>)</li>
<li>rls: propagate headers received in RLS response to backends (<a href="https://redirect.github.com/grpc/grpc-go/issues/5883">#5883</a>)</li>
</ul>
<h1>Bug Fixes</h1>
<ul>
<li>transport: drain client transport when streamID approaches MaxStreamID (<a href="https://redirect.github.com/grpc/grpc-go/issues/5889">#5889</a>)</li>
<li>server: after GracefulStop, ensure connections are closed when final RPC completes (<a href="https://redirect.github.com/grpc/grpc-go/issues/5968">#5968</a>)</li>
<li>server: fix a few issues where grpc server uses RST_STREAM for non-HTTP/2 errors (<a href="https://redirect.github.com/grpc/grpc-go/issues/5893">#5893</a>)</li>
<li>xdsclient: fix race which can happen when multiple load reporting calls are made at the same time. (<a href="https://redirect.github.com/grpc/grpc-go/issues/5927">#5927</a>)</li>
<li>rls: fix a data race involving the LRU cache (<a href="https://redirect.github.com/grpc/grpc-go/issues/5925">#5925</a>)</li>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
<li>gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
</ul>
<h1>Documentation</h1>
<ul>
<li>credentials/oauth: mark <code>NewOauthAccess</code> as deprecated (<a href="https://redirect.github.com/grpc/grpc-go/issues/5882">#5882</a>)
<ul>
<li>Special Thanks: <a href="https://github.com/buzzsurfr"><code>@​buzzsurfr</code></a></li>
</ul>
</li>
</ul>
<h2>Release 1.52.3</h2>
<h1>Bug Fixes</h1>
<ul>
<li>Fix user-agent version</li>
</ul>
<h2>Release 1.52.2</h2>
<h1>Bug Fixes</h1>
<ul>
<li>xds: fix panic involving double close of channel in xDS transport (<a href="https://redirect.github.com/grpc/grpc-go/issues/5959">#5959</a>)</li>
</ul>
<h2>Release 1.52.1</h2>
<h1>Bug Fixes</h1>
<ul>
<li>grpclb: rename grpclbstate package back to state (<a href="https://redirect.github.com/grpc/grpc-go/issues/5963">#5963</a>)</li>
</ul>
<h2>Release 1.52.0</h2>
<h1>New Features</h1>
<ul>
<li>xdsclient: log node ID with verbosity INFO (<a href="https://redirect.github.com/grpc/grpc-go/issues/5860">#5860</a>)</li>
<li>ringhash: impose cap on <code>max_ring_size</code> to reduce possibility of OOMs (<a href="https://redirect.github.com/grpc/grpc-go/issues/5801">#5801</a>)</li>
</ul>
<h1>Behavior Changes</h1>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-go/commit/dba26e15a07f43875ccf806a2dd6cbcbc1c12eab"><code>dba26e1</code></a> Change version to 1.53.0 (<a href="https://redirect.github.com/grpc/grpc-go/issues/5983">#5983</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/2a1e9348ff7b5d9f4b5039e84e6c9873b5b3e26e"><code>2a1e934</code></a> server: after GracefulStop, ensure connections are closed when final RPC comp...</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e2d69aa076dd070e3668784c4dc8bcf7131b3f67"><code>e2d69aa</code></a> tests: fix spelling of variable (<a href="https://redirect.github.com/grpc/grpc-go/issues/5966">#5966</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/a6376c9893f56fc3819bee9ef5d71f55cc2d38dd"><code>a6376c9</code></a> xds/resolver: cleanup tests to use real xDS client 3/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5953">#5953</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/bf8fc46fa6eb913e4ed0f6dee6c6a7b75e85fbf0"><code>bf8fc46</code></a> xds/resolver: cleanup tests to use real xDS client 5/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5955">#5955</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/3930549b38c0fc4cd94a95efccf7cef5f90515fd"><code>3930549</code></a> resolver: replace resolver.Target.Endpoint field with Endpoint() method (<a href="https://redirect.github.com/grpc/grpc-go/issues/5852">#5852</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/894816c487f8dd48fc971c45a7c5baa4b86ef7de"><code>894816c</code></a> grpclb: rename <code>grpclbstate</code> package back to <code>state</code> (<a href="https://redirect.github.com/grpc/grpc-go/issues/5962">#5962</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/e5a0237a46a5f95fa571624929be10c7afebb180"><code>e5a0237</code></a> encoding: fix duplicate compressor names (<a href="https://redirect.github.com/grpc/grpc-go/issues/5958">#5958</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/4adb2a7a00d8b62df5ea34d520fe3ca13bffd31a"><code>4adb2a7</code></a> xds/resolver: cleanup tests to use real xDS client 2/n (<a href="https://redirect.github.com/grpc/grpc-go/issues/5952">#5952</a>)</li>
<li><a href="https://github.com/grpc/grpc-go/commit/52a8392f374b8cd60e176b67925a7f8c1605d014"><code>52a8392</code></a> gcp/observability: update method name validation (<a href="https://redirect.github.com/grpc/grpc-go/issues/5951">#5951</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-go/compare/v1.47.0...v1.53.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=google.golang.org/grpc&package-manager=go_modules&previous-version=1.47.0&new-version=1.53.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:24:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4307" class=".btn">#4307</a>
            </td>
            <td>
                <b>
                    [Fix]: Provide a meaningful error for cert sanitization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit handles the error where the certificate sanitization procedure fails to construct the certificate chain due to misconfiguration. Before this commit, the peer will simply fail with panic without a clear explanation of what exactly was wrong.

Addresses (#4302).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 11:52:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4305" class=".btn">#4305</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: censorship monitor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- New feature

#### Description

BFT Block Puller: censorship monitor

- BFT header receivers that pull headers from the orderers, and keep the time and number of the last one.
- A BFT censorship monitor which compares the progress of headers relative to blocks, and triggers an alert if a header is ahead of the block stream for more than a certain time.

#### Related issues
#4306 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 08:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4304" class=".btn">#4304</a>
            </td>
            <td>
                <b>
                    Add SmartBFT consensus knobs to configtx.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The configtx.yaml now has the SmartBFT consensus knobs as in the Fabric samples

#### Related issues

https://github.com/hyperledger/fabric/issues/4295

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 08:03:54 +0000 UTC
    </div>
</div>

