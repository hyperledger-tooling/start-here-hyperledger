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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Allow custom peer images for test-network-k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Hyperledger provided Fabric peer images are only a sample so it would be good to make the k8s test network peer image configurable, for example to include a custom builder

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 14:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Provide clear guidance for debugging Java chaincode as a service #684
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **READY FOR MERGE** 

(This PR replaces PR #684, which lingered for too long in a DRAFT / review status, spanned multiple approaches, and had merge conflicts with the mainline.)



This PR addresses the need for a simple, clear example that illustrates the use of Chaincode-as-a-Service to build and run Java chaincode on a local development environment.

In addition, the README includes a section that describes how users may employ a Docker loopback interface to connect from a remote Peer binary to a local port on the host OS.  In this manner, chaincode may be run locally while attached to a debugger, with the peer running on a remote pod in Kubernetes.

In the first iteration of this PR, we introduced a new `ccpackage/*` folder to hold descriptive files that would be used to generate the chaincode-as-a-service package, AND help with the deployment to k8s: 

- ccpackage/metadata.json     (defines the package label)
- ccpackage/connection.json  (defines the CC service URL for gRPC access by the peer) 
- ccpackage/ccaas.json           (describes the CC name, used to construct the CC pods in k8s, and CC IMAGE) 

After community review, the PR has been reflected to *remove* the /ccpackage/ folder, opting to dynamically construct the cc package based on conventions and additional CLI arguments.  This has the benefit of applying directly to most (if not all) of the current sample code base, without introducing the crufty "ccaas" deployment descriptors for yet-another-deployment-technique-for-fabric.

A multi-phase Azure pipeline has been included to verify the overall approach for both golang and Java CCaaS asset transfer chaincode samples.

Some additional / loose ends that may warrant future PRs and improvements: 

- Additional testing on the `host.docker.internal` DNS alias is required (e.g. Win, Linux, revs of Docker, etc.) 

-  The doc sets up a flow with three installations of the same chaincode, but does not delete the chaincode between steps.  (How does one _delete_ a chaincode, btw?) 

-  file-based arguments must all be absolute paths. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 13:10:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Bump nconf from 0.11.3 to 0.11.4 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [nconf](https://github.com/flatiron/nconf) from 0.11.3 to 0.11.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/flatiron/nconf/releases">nconf's releases</a>.</em></p>
<blockquote>
<h2>v0.11.4</h2>
<p>Fixes:</p>
<ul>
<li>Prevent improper usage of the memory store from polluting the object prototype (<a href="https://github-redirect.dependabot.com/flatiron/nconf/issues/397">#397</a>) (<a href="https://github.com/mhamann"><code>@​mhamann</code></a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/indexzero/nconf/commit/f25feb2913fc21a5d80039f6213c2d9ae906ec29"><code>f25feb2</code></a> 0.11.4</li>
<li><a href="https://github.com/indexzero/nconf/commit/2e9e4538a8b9c33dabdafd8ec1dc6064fac9d070"><code>2e9e453</code></a> chore: disable package-lock, since this is a lib</li>
<li><a href="https://github.com/indexzero/nconf/commit/7aa94020e493eca482239492d0126d63b1ce2630"><code>7aa9402</code></a> chore: update node version test matrix</li>
<li><a href="https://github.com/indexzero/nconf/commit/feaba562b812b21215897f71b0c8b3bf39cf8d7d"><code>feaba56</code></a> fix(security): prevent prototype pollution in memory store (<a href="https://github-redirect.dependabot.com/flatiron/nconf/issues/397">#397</a>)</li>
<li>See full diff in <a href="https://github.com/flatiron/nconf/compare/v0.11.3...v0.11.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nconf&package-manager=npm_and_yarn&previous-version=0.11.3&new-version=0.11.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-04-22 23:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    Use maven central for gateway client dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the release-1.4 commercial paper client applications to pull the gateway jars from Maven central.

This PR supersedes PR #585 (abandoned / closed) 
    
Signed-off-by: lyd <luoyaodong98@gmail.com>

Co-authored-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 14:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Remove kubectl binary (again)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since kubectl binary is mistakenly added again in PR #714, this patch removes it.

It seems that the following commit was mixed up with another PR commits, including PR #713.
https://github.com/hyperledger/fabric-samples/pull/714/commits/24c296c8a8e6966595c6395bcc4ba9948217176a
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 02:15:30 +0000 UTC
    </div>
</div>

