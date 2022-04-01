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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    Fix Linting: Add in a `-not -path` option to find 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix errors like this that occur from time to time..
```
Linting ./.git/refs/remotes/origin/dependabot/npm_and_yarn/asset-transfer-basic/rest-api-typescript
~/work/1/s/.git/refs/remotes/origin/dependabot/npm_and_yarn/asset-transfer-basic/rest-api-typescript ~/work/1/s
```




Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 09:13:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/698" class=".btn">#698</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-03-31 21:39:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Updates the README and documentation guide for the Kube test network's usage of Nginx ingress
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a documentation update associated with a fix for Issue #685 

The updates associated with this doc update are described in PR #692 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 18:21:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    CORS Enablement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After feedback from the community, this PR adds CORS support in, but as an option
to enable.

Along with warnings that the default wildcard origin might not be applicable
in a production use case

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 16:55:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/694" class=".btn">#694</a>
            </td>
            <td>
                <b>
                    fix chaincode breakage in asset-transfer-basic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                only broken in main branch, not in release-2.2

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 16:36:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/693" class=".btn">#693</a>
            </td>
            <td>
                <b>
                    [release-2.2] Missing await in asset-transfer-basic chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Missing an `await` on the asset-transfer-basic javascript chaincode.

This has been fixed in the main branch but needs to be fixed in the
release-2.2 branch

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:38:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    test-network-k8s : Connect to Fabric services via Nginx Ingress - READY FOR MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the Kube test network to access Fabric services via an Ingress controller.  This allows for easy access to the CAs, peers, orderers, and load-balanced Gateway Peer via the nginx bound to localhost:443.

In previous iterations, any administration of the network involved a remote exec to execute commands on an "admin CLI pod" running in the cluster.  In addition, any time files needed to get to/from the volume mounts in Kubernetes, an overly complicated sequence of arcane `exec tar --.... ` commands was necessary.

With this PR, the network is instantiated, exposing core services at the *.vcap.me (wildcard match to 127.0.0.1) DNS domain.  Fabric binaries are run directly on the host, and certificate enrollments are managed locally as if they were maintained in a local wallet storage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 15:14:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Update the REST Example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. For development purposes CORS can hinder testing examples. Therefore enable CORS if needed, default off
2. The default chaincode use Capitalized JSON Names, whereas for new asset the REST validation didn't.. Adjusted
so it matches the chaincode

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 12:25:18 +0000 UTC
    </div>
</div>

