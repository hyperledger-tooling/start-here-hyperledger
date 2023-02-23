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
                PR <a href="https://github.com/hyperledger/fabric/pull/4064" class=".btn">#4064</a>
            </td>
            <td>
                <b>
                    BFT review comments: channelparticipation.Join
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I92a347a6105fbe99e934f8d4686378e58eb984ce


#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Addressing review comments on the modification of channelparticipation.Join in the BFT commit.

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-23 14:17:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4058" class=".btn">#4058</a>
            </td>
            <td>
                <b>
                    Address comments on BFT PR
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
        Created At 2023-02-21 14:45:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4057" class=".btn">#4057</a>
            </td>
            <td>
                <b>
                    Async connections to endpoints (backport #4050)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4050 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-21 08:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4056" class=".btn">#4056</a>
            </td>
            <td>
                <b>
                    Async connections to endpoints (backport #4050)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4050 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-21 08:33:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4055" class=".btn">#4055</a>
            </td>
            <td>
                <b>
                    Revert github.com/prometheus/client_golang to v1.11.1 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The bump to v1.14.0 causes Fabric compilation issues on ubuntu docker images.
See issue #4052 for details about the problematic build tag.
For now, it is acceptable to revert to v1.11.1 where there is no such build tag.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 21:41:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4054" class=".btn">#4054</a>
            </td>
            <td>
                <b>
                    Revert github.com/prometheus/client_golang to v1.11.1 (main)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The bump to v1.14.0 causes Fabric compilation issues on ubuntu docker images.
See issue hyperledger#4052 for details about the problematic build tag.
For now, it is acceptable to revert to v1.11.1 where there is no such build tag.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 21:37:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4051" class=".btn">#4051</a>
            </td>
            <td>
                <b>
                    Gateway with BFT integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add integration test to gateway suite for transaction submission to BFT ordering service. Change gateway handling of “request already exists” error to treat it as a success, allowing the client to re-submit using the same txID.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 17:14:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4050" class=".btn">#4050</a>
            </td>
            <td>
                <b>
                    Async connections to endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add the AsyncConnect flag to the grpc connection code for gateway connections to endorsing peers and orderers

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 15:46:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4048" class=".btn">#4048</a>
            </td>
            <td>
                <b>
                    Use local peer ledger height from ledger instead of discovery in Gateway (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of 969040c6a7028117c8284652b73813410decf059 from main branch.

Discovery ledger heights can be slightly behind the actual peer ledger height. Ensure the most up-to-date information is used for the local peer by querying the ledger height directly. This avoids the possibility of a remote peer with a lower ledger height being selected as an endorser.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 10:53:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4047" class=".btn">#4047</a>
            </td>
            <td>
                <b>
                    Use local peer ledger height from ledger instead of discovery in Gateway (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of 969040c6a7028117c8284652b73813410decf059 from main branch.

Discovery ledger heights can be slightly behind the actual peer ledger height. Ensure the most up-to-date information is used for the local peer by querying the ledger height directly. This avoids the possibility of a remote peer with a lower ledger height being selected as an endorser.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 10:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4045" class=".btn">#4045</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net to v0.7.0 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump golang.org/x/net to v0.7.0.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 16:27:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4044" class=".btn">#4044</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.5.0 to 0.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.5.0 to 0.7.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/8e2b117aee74f6b86c207a808b0255de45c0a18a"><code>8e2b117</code></a> http2/hpack: avoid quadratic complexity in hpack decoding</li>
<li><a href="https://github.com/golang/net/commit/547e7edf3873d6f3a9c093d3785f9e2289e00746"><code>547e7ed</code></a> http2: avoid referencing ResponseWrite.Write parameter after returning</li>
<li><a href="https://github.com/golang/net/commit/39940adcaaa73e661124cb80fb8dd57ea929dbaf"><code>39940ad</code></a> html: parse comments per HTML spec</li>
<li><a href="https://github.com/golang/net/commit/87ce33ecb484cbb6bcfc8e506ce0330ef72e0847"><code>87ce33e</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/415cb6d518e71d202e2dc2f44c475cbff84eee72"><code>415cb6d</code></a> all: fix some comments</li>
<li><a href="https://github.com/golang/net/commit/7e3c19ca52e202ae203b1914fc00c8e47a4d72fa"><code>7e3c19c</code></a> all: correct typos in comments</li>
<li><a href="https://github.com/golang/net/commit/296f09aa3817abc1ddff7703799bf9babb7bbd16"><code>296f09a</code></a> http2: case insensitive handling for 100-continue</li>
<li><a href="https://github.com/golang/net/commit/f8411da775a685be247bbedcb3ed2c998f895cd2"><code>f8411da</code></a> nettest: fix tests on dragonfly and js/wasm</li>
<li>See full diff in <a href="https://github.com/golang/net/compare/v0.5.0...v0.7.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.5.0&new-version=0.7.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-02-17 16:11:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4043" class=".btn">#4043</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update release notes and doc for v2.2.10.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 15:38:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4041" class=".btn">#4041</a>
            </td>
            <td>
                <b>
                    Refactor of Gateway code (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of https://github.com/hyperledger/fabric/commit/11896ae6e0dfa89bb475d0311192e718a4921ffe from main branch, keeping structure in step between branches.

Split some code into separate files. Particularly the gRPC service method implementation and tests were unreasonably large, making the codebase difficult to navigate and extend. Code that was previously in api.go is now located in: chaincodeevents.go, commitstatus.go, diff.go, endorse.go, evaluate.go, and submit.go. Unit tests specific to these functions are split out of api_test.go into corresponding _test.go files.

Simplification of the way chaincode events unit tests define the local peer ledger height. Previously a postSetup function for specific tests reconfigured the ledger mocks. Now only a localLedgerHeight property is specified in the test definition.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 11:03:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4040" class=".btn">#4040</a>
            </td>
            <td>
                <b>
                    Refactor of Gateway code (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of 11896ae6e0dfa89bb475d0311192e718a4921ffe from main branch, keeping structure in step between branches.

Split some code into separate files. Particularly the gRPC service method implementation and tests were unreasonably large, making the codebase difficult to navigate and extend. Code that was previously in api.go is now located in: chaincodeevents.go, commitstatus.go, diff.go, endorse.go, evaluate.go, and submit.go. Unit tests specific to these functions are split out of api_test.go into corresponding _test.go files.

Simplification of the way chaincode events unit tests define the local peer ledger height. Previously a postSetup function for specific tests reconfigured the ledger mocks. Now only a localLedgerHeight property is specified in the test definition.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 11:00:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4039" class=".btn">#4039</a>
            </td>
            <td>
                <b>
                    Add workflow_dispatch option for release action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Older release branches such as release-2.2 have a release action that gets triggered based on a manual workflow_dispatch. 
The 'main' branch must also have workflow_dispatch enabled in order to trigger the release action on specific release branches.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 09:56:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4038" class=".btn">#4038</a>
            </td>
            <td>
                <b>
                    Home Button and Text of Side Navigation Menu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The "Home Button" and "Text" in the side nav is not visible. It is set as "color: transparent". I edited it to "color: White".

**Before** : 
![SS1](https://user-images.githubusercontent.com/71092045/219601271-990e416f-3693-4261-bf62-c7c4671b335b.png)

----------------------------------------------------------                           ----------------------------------------------------------------
**After** :
![SS2](https://user-images.githubusercontent.com/71092045/219601793-92934b41-bbd2-40c7-be87-70b9558aa72c.png)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 09:11:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4037" class=".btn">#4037</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.5.16 to 1.5.18 (backport #4031)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4031 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 03:54:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4036" class=".btn">#4036</a>
            </td>
            <td>
                <b>
                    Disable fail-fast for integration test suite matrix (backport #4030) (backport #4035)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4035 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 03:53:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4035" class=".btn">#4035</a>
            </td>
            <td>
                <b>
                    Disable fail-fast for integration test suite matrix (backport #4030)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4030 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 02:34:36 +0000 UTC
    </div>
</div>

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

