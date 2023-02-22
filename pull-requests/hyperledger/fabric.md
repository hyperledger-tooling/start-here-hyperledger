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

