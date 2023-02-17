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
                PR <a href="https://github.com/hyperledger/fabric/pull/4034" class=".btn">#4034</a>
            </td>
            <td>
                <b>
                    Fix purge private data integration test flake
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prior test restarted peers.
Need to make sure all peers are up and connected before continuing to next test.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 21:22:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4033" class=".btn">#4033</a>
            </td>
            <td>
                <b>
                    Bump github.com/prometheus/client_golang to v1.11.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note that client_golang v1.11.1 attempts pull in protobuf v1.4.3.
However, protobuf v1.4.3 is incompatible with raft in v2.2.x.
Therefore, need to add a "replace" in go.mod to keep protobuf at v1.3.3.

The update also pulls in github.com/go-kit/kit v0.9.0, which requires one code update.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 19:52:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4032" class=".btn">#4032</a>
            </td>
            <td>
                <b>
                    Refactor of Gateway code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split some code into separate files. Particularly the gRPC service method implementation and tests were unreasonably large, making the codebase difficult to navigate and extend. Code that was previously in api.go is now located in: chaincodeevents.go, commitstatus.go, diff.go, endorse.go, evaluate.go, and submit.go. Unit tests specific to these functions are split out of api_test.go into corresponding _test.go files.

Simplification of the way chaincode events unit tests define the local peer ledger height. Previously a postSetup function for specific tests reconfigured the ledger mocks. Now only a localLedgerHeight property is specified in the test definition.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 16:13:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4031" class=".btn">#4031</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.5.16 to 1.5.18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/containerd/containerd](https://github.com/containerd/containerd) from 1.5.16 to 1.5.18.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/containerd/containerd/releases">github.com/containerd/containerd's releases</a>.</em></p>
<blockquote>
<h2>containerd 1.5.18</h2>
<p>Welcome to the v1.5.18 release of containerd!</p>
<p>The eighteenth patch release for containerd 1.5 includes fixes for CVE-2023-25153 and CVE-2023-25173
along with a security update for Go.</p>
<h3>Notable Updates</h3>
<ul>
<li><strong>Fix supplementary groups not being set up properly</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-hmfx-3pcx-653p">GHSA-hmfx-3pcx-653p</a>)</li>
<li><strong>Fix OCI image importer memory exhaustion</strong> (<a href="https://github.com/containerd/containerd/security/advisories/GHSA-259w-8hf6-59c2">GHSA-259w-8hf6-59c2</a>)</li>
<li><strong>Update Go to 1.19.6</strong> (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8112">#8112</a>)</li>
</ul>
<p>See the changelog for complete list of changes</p>
<p>Please try out the release binaries and report any issues at
<a href="https://github.com/containerd/containerd/issues">https://github.com/containerd/containerd/issues</a>.</p>
<h3>Contributors</h3>
<ul>
<li>Akihiro Suda</li>
<li>Derek McGowan</li>
<li>Ye Sijun</li>
<li>Samuel Karp</li>
<li>Phil Estes</li>
<li>Swagat Bora</li>
<li>Wei Fu</li>
</ul>
<h3>Changes</h3>
<!-- raw HTML omitted -->
<ul>
<li>[release/1.5] Prepare release notes for v1.5.18 (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8117">#8117</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/ddf9de6cbb30f9edf1b04d304eac67d1383e406b"><code>ddf9de6cb</code></a> Prepare release notes for v1.5.18</li>
</ul>
</li>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-hmfx-3pcx-653p">GHSA-hmfx-3pcx-653p</a>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/a62c38bf2173faa813018939710fc8491e4f7dba"><code>a62c38bf2</code></a> oci: fix additional GIDs</li>
<li><a href="https://github.com/containerd/containerd/commit/3b89da580b76471d6c03cb1fc6c14db6aa23d3db"><code>3b89da580</code></a> oci: fix loop iterator aliasing</li>
<li><a href="https://github.com/containerd/containerd/commit/b07ec6b251bd51f06bc72ef408f31e3f6e6e87f9"><code>b07ec6b25</code></a> oci: skip checking gid for WithAppendAdditionalGroups</li>
<li><a href="https://github.com/containerd/containerd/commit/356672cb56fd5a0eed11e5089ac824c7ab09ffac"><code>356672cb5</code></a> refactor: reduce duplicate code</li>
<li><a href="https://github.com/containerd/containerd/commit/6a7b7617cfbd90009a2e05e0e5eff4ef92028d7b"><code>6a7b7617c</code></a> add WithAdditionalGIDs test</li>
<li><a href="https://github.com/containerd/containerd/commit/832bcf300b1ec29c9b08326aab2d4eafee58dd85"><code>832bcf300</code></a> add WithAppendAdditionalGroups helper</li>
</ul>
</li>
<li>Github Security Advisory <a href="https://github.com/containerd/containerd/security/advisories/GHSA-259w-8hf6-59c2">GHSA-259w-8hf6-59c2</a>
<ul>
<li><a href="https://github.com/containerd/containerd/commit/19a347e456f3ab66909edca5351aa6f4ed1be177"><code>19a347e45</code></a> importer: stream oci-layout and manifest.json</li>
</ul>
</li>
<li>[release/1.5] Go 1.19.6 (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8112">#8112</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc243</code></a> Go 1.19.6</li>
</ul>
</li>
<li>[release/1.5] Fix retry logic within devmapper device deactivation (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8089">#8089</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d045d</code></a> Fix retry logic within devmapper device deactivation</li>
</ul>
</li>
<li>[release/1.5] CI: skip some jobs when <code>repo != containerd/containerd</code> (<a href="https://github-redirect.dependabot.com/containerd/containerd/pull/8084">#8084</a>)
<ul>
<li><a href="https://github.com/containerd/containerd/commit/34451bc66453aad2f911aa8bffa6817061e4a72b"><code>34451bc66</code></a> CI: skip some jobs when <code>repo != containerd/containerd</code></li>
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
<li><a href="https://github.com/containerd/containerd/commit/39bb06f98f17c7a226b10269d325c861585b2389"><code>39bb06f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8117">#8117</a> from dmcgowan/prepare-v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/ddf9de6cbb30f9edf1b04d304eac67d1383e406b"><code>ddf9de6</code></a> Prepare release notes for v1.5.18</li>
<li><a href="https://github.com/containerd/containerd/commit/28e461805038a431c0bd1c04f31a438470c24450"><code>28e4618</code></a> Merge pull request from GHSA-hmfx-3pcx-653p</li>
<li><a href="https://github.com/containerd/containerd/commit/959e1cf9602f3b7a71bdca7b6344b40e00504730"><code>959e1cf</code></a> Merge pull request from GHSA-259w-8hf6-59c2</li>
<li><a href="https://github.com/containerd/containerd/commit/b4538c253204b169366b7f3d3f990b47eae7ade0"><code>b4538c2</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8112">#8112</a> from AkihiroSuda/cherrypick-8109-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/4209dc243005af926fbd0382cbd6cf4cd26beeef"><code>4209dc2</code></a> Go 1.19.6</li>
<li><a href="https://github.com/containerd/containerd/commit/7c3b24362756e11c841ec7fa4a8aecb8f94e6894"><code>7c3b243</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8089">#8089</a> from swagatbora90/backport-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/0d16d045dfd0d800a00dc362736b815f6cc96de8"><code>0d16d04</code></a> Fix retry logic within devmapper device deactivation</li>
<li><a href="https://github.com/containerd/containerd/commit/9e9f4c8ea77d016387bee13eeb773f4a79d6c054"><code>9e9f4c8</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/containerd/containerd/issues/8084">#8084</a> from AkihiroSuda/ci-skip-on-fork-1.5</li>
<li><a href="https://github.com/containerd/containerd/commit/a62c38bf2173faa813018939710fc8491e4f7dba"><code>a62c38b</code></a> oci: fix additional GIDs</li>
<li>Additional commits viewable in <a href="https://github.com/containerd/containerd/compare/v1.5.16...v1.5.18">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/containerd/containerd&package-manager=go_modules&previous-version=1.5.16&new-version=1.5.18)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 14:39:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4030" class=".btn">#4030</a>
            </td>
            <td>
                <b>
                    Disable fail-fast for integration test suite matrix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allowing all suites to run to completion minimises the impact of test flakes. Only failing suites need to be re-run rather then re-running the entire integration test suite.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 14:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4029" class=".btn">#4029</a>
            </td>
            <td>
                <b>
                    Backport of Performance Considerations topic to 2.5
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

Backport from Main of Performance Considerations topic

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 13:59:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4028" class=".btn">#4028</a>
            </td>
            <td>
                <b>
                    Use local peer ledger height from ledger instead of discovery in Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Discovery ledger heights can be slightly behind the actual peer ledger height. Ensure the most up-to-date information is used for the local peer by querying the ledger height directly. This avoids the possibility of a remote peer with a lower ledger height being selected as an endorser.

Refactored Gateway service method implementations and associated tests into separate files as the size of the api files were getting unmanageable.

Closes hyperledger/fabric-gateway#558
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 13:17:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4027" class=".btn">#4027</a>
            </td>
            <td>
                <b>
                    Bump dependencies (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains 4 commits that can be reviewed individually:

Bump golang.org/x/net/http2 to v0.5.0 (release-2.2)
Bump golang.org/x/text/language to v0.7.0 (release-2.2)
Bump github.com/opencontainers/image-spec to v1.0.2 (release-2.2)
Update go.mod version to 1.18 (release-2.2)

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 04:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4026" class=".btn">#4026</a>
            </td>
            <td>
                <b>
                    Remainder of Performance considerations edit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Edited starting with "Orderer considerations" continuing through end: 
- Note in places we say collecting "enough" signatures - are there some cases where a specific signature is required in addition to number. 
- It may be useful to indicate how much better Go is than Node for performance, if they are close or not close.

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

- Documentation update

#### Description

new doc, per request

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
        Created At 2023-02-14 21:47:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4025" class=".btn">#4025</a>
            </td>
            <td>
                <b>
                    Bump prometheus/client_golang to v1.14.0 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump prometheus/client_golang to v1.14.0.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 17:59:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4024" class=".btn">#4024</a>
            </td>
            <td>
                <b>
                    Orderer v3: prevent bootstrap with system channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I04947477982f0039366b7cc3ba08ce2f916c9d49

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: prevent bootstrap with system channel

#### Related issues
Issue: #4020 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 15:26:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4022" class=".btn">#4022</a>
            </td>
            <td>
                <b>
                    Edits up to Orderer considerations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Probably best to provide updates piecemeal for commentary or change of direction etc. - done up until the start of "Orderer considerations" section. 

- Can "runaway situations" be described more precisely, formally.. 
- We use "you" a lot so let's ensure that we always mean the same or similar role / authorization for the action. 
- To be continued with a subsequent PR. 


Signed-off-by: Josh Horton <joshh@us.ibm.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

Per request, see the PR for details.

#### Additional details

To be continued next with Orderer considerations section.

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
        Created At 2023-02-13 21:31:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4021" class=".btn">#4021</a>
            </td>
            <td>
                <b>
                    Bump prometheus/client_golang to v1.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump prometheus/client_golang to v1.14.0

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 19:30:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4018" class=".btn">#4018</a>
            </td>
            <td>
                <b>
                    ledgerutil: Add "verify" command
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

We would like to propose a new command in Ledger Utility that checks the integrity of a single ledger. The existing commands in Ledger Utility aim at checking the ledger when any difference is found by comparing two ledgers. The purpose of the command proposed is to complement these commands by finding any defect in ledger files in a single peer that could be caused by potential software bugs or disk errors.

This patch adds a new command, “verify,” to Ledger Utility, which performs integrity checks for a specified ledger. Currently, the checks for the hash values in the headers of the blocks are implemented.

A use case assumed is to run the command locally in a peer periodically, which can be utilized as one of the health checks for the peer.

#### Additional details

This patch contains a sample ledger that is tweaked to have a hash value error (the hash value for Block 0 is modified not to match the block payload). Using the ledger, the command proposed can detect the error as follows:

```
$ ./build/bin/ledgerutil verify ./internal/ledgerutil/testdata/sample_bad_ledger -o /tmp/ledgerutil-verify-result-bad
...
Successfully executed verify tool. Some error(s) are found.
$ cat /tmp/ledgerutil-verify-result-bad/mychannel_verification_result/blocks.json
[
{"number":0,"valid":false,"errors":["DataHash mismatch"]}
,
{"number":1,"valid":false,"errors":["PreviousHash mismatch"]}
]
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 09:33:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4017" class=".btn">#4017</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: raft no.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I18cb92f0af7b9d4fa700da87368484bd26ab5345

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: raft no.4
- raft: channel participation tests
- nwo: network tests
- some cleanup

#### Related issues

Issue: #3515 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 14:10:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4014" class=".btn">#4014</a>
            </td>
            <td>
                <b>
                    Return channel header on missing system channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement (improvement to log)

#### Description

Currently, It fails to report the channel name in
the log as it failed to return the channel header
to the caller.

#### Additional details

> 2023-02-08 23:07:45.078 UTC 138d WARN [orderer.common.broadcast] ProcessMessage -> **[channel: unknown]** Could not get message processor for serving 10.244.0.9:33422: channel creation request not allowed because the orderer system channel is not defined

It failed to report the channel name when it failed to locate the channel. As shown in the above log `**[channel: unknown]**`

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 11:20:31 +0000 UTC
    </div>
</div>

