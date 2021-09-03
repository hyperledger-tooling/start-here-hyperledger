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
                PR <a href="https://github.com/hyperledger/fabric/pull/2889" class=".btn">#2889</a>
            </td>
            <td>
                <b>
                    Fix process termination waits in health tests (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #1563

The current code is passing a function to `Eventually` that returns a
channel instead of the channel to wait on.

Signed-off-by: Matthew Sykes <sykesmat@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 21:13:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2888" class=".btn">#2888</a>
            </td>
            <td>
                <b>
                    platform/golang: loosen assertion for Go 1.16.2 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The error messages for commands executed outside of a module were
changed in Go 1.16.2. This change loosens our assertion to handle the
old and new messages.
    
Signed-off-by: Matthew Sykes <sykesmat@us.ibm.com>
Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 15:50:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2887" class=".btn">#2887</a>
            </td>
            <td>
                <b>
                    platform/golang: loosen assertion for Go 1.16.2 (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The error messages for commands executed outside of a module were
changed in Go 1.16.2. This change loosens our assertion to handle the
old and new messages.
    
Signed-off-by: Matthew Sykes <sykesmat@us.ibm.com>
Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 15:44:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2886" class=".btn">#2886</a>
            </td>
            <td>
                <b>
                    deps: bump testify (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #2336 for Go 1.16 tests.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 15:28:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2885" class=".btn">#2885</a>
            </td>
            <td>
                <b>
                    deps: bump testify (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #2336 for Go 1.16 tests.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 15:21:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2882" class=".btn">#2882</a>
            </td>
            <td>
                <b>
                    Fixed a typo in private_data_tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: realnimish <realnimish@gmail.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

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
        Created At 2021-08-30 22:42:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2881" class=".btn">#2881</a>
            </td>
            <td>
                <b>
                    Update alpine base image to 3.14
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update alpine base image to 3.14

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 20:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2880" class=".btn">#2880</a>
            </td>
            <td>
                <b>
                    Update x509.CertPool equality checks (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go 1.16 changed the CertPool implementation to employ functions to
lazily acquire certificates. This change effectively breaks
`reflect.DeepEqual` used by our test assertions.

This commit changes the assertions compare certificate subjects instead
of the entire pool. While not the same, it's a close approximation.

See https://go-review.googlesource.com/c/go/+/229917

Signed-off-by: Matthew Sykes <sykesmat@us.ibm.com>
Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 20:21:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2879" class=".btn">#2879</a>
            </td>
            <td>
                <b>
                    Update x509.CertPool equality checks (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go 1.16 changed the CertPool implementation to employ functions to
lazily acquire certificates. This change effectively breaks
`reflect.DeepEqual` used by our test assertions.

This commit changes the assertions compare certificate subjects instead
of the entire pool. While not the same, it's a close approximation.

See https://go-review.googlesource.com/c/go/+/229917

Signed-off-by: Matthew Sykes <sykesmat@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 20:15:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2878" class=".btn">#2878</a>
            </td>
            <td>
                <b>
                    Clean up Go modules (main)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run "go mod tidy" and "go mod vendor" on main.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 17:24:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2877" class=".btn">#2877</a>
            </td>
            <td>
                <b>
                    Update Go to v1.16.7 and alpine to 3.14 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go module support is assumed starting in Go v1.16.

Therefore, for chaincodes without go modules (such as in the integration tests),
need to explicitly set GO111MODULE to off otherwise chaincode will not compile.
See Go v1.16 release notes for more details: https://golang.org/doc/go1.16#go-command

As part of troubleshooting the Go upgrade, also added debug for the chaincode
compile command.

Also update alpine to 3.14.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 17:07:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2876" class=".btn">#2876</a>
            </td>
            <td>
                <b>
                    Clean up Go modules (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run "go mod tidy" to clean up module dependencies in release-2.2.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 16:58:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2875" class=".btn">#2875</a>
            </td>
            <td>
                <b>
                    Clean up Go modules (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run "go mod tidy" to clean up module dependencies in release-2.3

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 16:51:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2874" class=".btn">#2874</a>
            </td>
            <td>
                <b>
                    Update Go to v1.16.7 and alpine to 3.14 (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update Go to v1.16.7.
Go module support is assumed starting in Go v1.16.
Therefore, for chaincodes without go modules (such as in the integration tests),
need to explicitly set GO111MODULE to off otherwise chaincode will not compile.
See Go v1.16 release notes for more details: https://golang.org/doc/go1.16#go-command

As part of troubleshooting the Go upgrade, also added debug for the chaincode
compile command.

Also update alpine to 3.14.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 16:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2873" class=".btn">#2873</a>
            </td>
            <td>
                <b>
                    Change name of test network docker network in 2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@triplepointliquidity.com>

A PR in the Fabric samples recently changed the name of the Fabric test network docker network from `net_test` to `fabric_test`. This PR updates the documentation to match.

#### Type of change

- Documentation update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 16:24:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2868" class=".btn">#2868</a>
            </td>
            <td>
                <b>
                    Stop spamming for wait channel acquirement in orderer integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #2863

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-28 21:17:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2867" class=".btn">#2867</a>
            </td>
            <td>
                <b>
                    [Document] typo fix on BlockHashingDataStructure and HashingAlgorithm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: DavidLiu <david.yx.liu@oracle.com>

#### Type of change

- Documentation update

#### Description

Now beyond SHA256, SHA3_256 is also supported HashingAlgorithm
BlockHashingDataStructure --> BlockDataHashingStructure



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-28 14:47:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2865" class=".btn">#2865</a>
            </td>
            <td>
                <b>
                    Stop spamming for wait channel acquirement in orderer integration test (backport #2863)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2863 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-28 11:32:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2864" class=".btn">#2864</a>
            </td>
            <td>
                <b>
                    Stop spamming for wait channel acquirement in orderer integration test (backport #2863)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2863 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-28 11:31:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2863" class=".btn">#2863</a>
            </td>
            <td>
                <b>
                    Stop spamming for wait channel acquirement in orderer integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The code passes a function that returns a channel instead of the channel returned by that function.
As a result, the function is being polled thousands of times needlessly and thousands of channels
are being created, after which a goroutine per channel feeds a value into each of them.

Unfortunately, Gomega uses reflection based select on each of these channels, which is non-blocking,
meaning it just grabs a lock on the channel, and if the sender goroutine hasn't sent the item yet,
it returns false.

Since we pass in the Gomega.Eventually, a function (and not a channel), the reflection based receive is only attempted
once on each channel (out of the thousands created) and this creates a flake, because sometimes
we reach the timeout before one of the goroutines has a chance to obtain the lock on the channel
before the reflection based select obtains it, sees the channel buffer is empty, and the Gomega
attempt for that channel is then given up.

Resolves #2860 

Change-Id: I4417703d17e48afec50f46f3ae6b77a8e61a9be7
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 23:06:50 +0000 UTC
    </div>
</div>

