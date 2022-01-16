---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.6 to 1.14.7 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.6 to 1.14.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ede36d7c60d3acdcd324dcd99a9dbd52e4fb3a6"><code>2ede36d</code></a> Release version 1.14.7 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8b347cbcef7c7b72a6e9be20f5710c17d6163c22"><code>8b347cb</code></a> Drop Cookie header across domains.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.6...v1.14.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.6&new-version=1.14.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-16 01:03:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/583" class=".btn">#583</a>
            </td>
            <td>
                <b>
                    peer address export
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                environment variable should be exported to take effect i guess...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 16:53:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/582" class=".btn">#582</a>
            </td>
            <td>
                <b>
                    Added 'jq' to prerequisite script and readme for k8s test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New pull as per suggestion given on #581 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 16:16:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    Bug fix in samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added missing grpc dependency in package.json
Included migrated application in ci pipelines

Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 13:23:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/576" class=".btn">#576</a>
            </td>
            <td>
                <b>
                    Add prometheus/grafana performances sample in test-network directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add the ability to separate start a prometheus and grafana server either in the fabric docker network test or as a separate network
- provide a sample prometheus configuration that connects to the fabric test network to collect metrics
- provide a sample grafana dashboard to collect some of the more interesting statistics
- provide a README explaining how to setup this environment
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 11:54:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/575" class=".btn">#575</a>
            </td>
            <td>
                <b>
                    Update REST sample readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move signposts to sample source files from index.ts to the readme and reinforce the key aspects of the sample

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 17:28:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/574" class=".btn">#574</a>
            </td>
            <td>
                <b>
                    Private data samples migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-10 13:17:14 +0000 UTC
    </div>
</div>

