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

Change-Id: I4417703d17e48afec50f46f3ae6b77a8e61a9be7
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 23:06:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    Private Data Comparison
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2818

Signed-off-by: Julian Castrence <juliancastrence@ibm.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature
- Improvement (improvement to code, performance, etc)

#### Description

- Compare command now generates a list of differences between the private data in a separate json output file.

<!--- Describe your changes in detail, including motivation. -->



<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

- [fabric #2818](https://app.zenhub.com/workspaces/fabric-57c43689b6f3d8060d082cf1/issues/hyperledger/fabric/2818)

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
        Created At 2021-08-27 01:55:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2859" class=".btn">#2859</a>
            </td>
            <td>
                <b>
                    Nominate Andrew Coleman as Fabric maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I would like to nominate Andrew Coleman as a Fabric maintainer.
Andrew has many years experience with Fabric, especially Fabric
SDKs where he has been a maintainer and lead developer.
Last year, Andrew demonstrated his Go expertise while working
on the fabric-sdk-go contract programming model.
In the past year Andrew has been working in the core Fabric
repository, leading the Fabric Gateway feature from RFC and community
discussions through implementation, test, and a successful beta preview.
Andrew has also picked up skill in other areas of the peer, and
has been reviewing PRs, extending tests, and coaching others.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 17:54:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2858" class=".btn">#2858</a>
            </td>
            <td>
                <b>
                     Options for GRPC message size configurable (backport #2805) 1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of pull request #2805

Signed-off-by: Parameswaran Selvam parselva@in.ibm.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 16:03:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2857" class=".btn">#2857</a>
            </td>
            <td>
                <b>
                    Implement DisregardNamespacePolicy for gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for the ‘DisregardNamespacePolicy’ flag when generating the ChaincodeInterest structure in the transaction simulator.

resolves #2856 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 15:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2855" class=".btn">#2855</a>
            </td>
            <td>
                <b>
                    Clarify bootstrap.sh message when fabric-samples tag not found
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The latest versions of fabric are not tagged in fabric-samples repository.
This is so that users that are using the download script
and trying the most recent Fabric versions will
automatically get the latest samples improvements/fixes, rather
than getting an old tagged version of the samples.
This works since the maintainers try to keep recent versions
of Fabric compatible with latest fabric-samples.
If there is an incompatibility introduced (e.g. the switch to
osnadmin in v2.3), at that point the maintainers tag
fabric-samples to align with Fabric versions (e.g.
v2.2.3 Fabric works with v2.2.3 of samples without osnadmin use).
This commit simply improves the message that download
script users receive so that they know that using the
fabric-samples main branch is acceptable.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 19:36:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2854" class=".btn">#2854</a>
            </td>
            <td>
                <b>
                    Gateway integration tests - adv. endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added extra integration tests to the gateway suite to verify the automatic generation of the ChaincodeInterest structure is working as expected. In particular the following areas have been added:

- Submitting transactions that modify an SBE state.
- Submitting transactions that modify a private data collection.
- Submitting transactions involving chaincode to chaincode calls.

resolves #2853 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 13:57:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2851" class=".btn">#2851</a>
            </td>
            <td>
                <b>
                    Prepare for next release v2.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare Makefile and release notes for next release v2.4.0.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 20:45:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2850" class=".btn">#2850</a>
            </td>
            <td>
                <b>
                    Update Go to v1.16.7
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

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 12:16:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2849" class=".btn">#2849</a>
            </td>
            <td>
                <b>
                    Options for GRPC message size configurable (backport #2805) 2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of pull request #2805

Signed-off-by: Parameswaran Selvam parselva@in.ibm.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-22 14:40:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2848" class=".btn">#2848</a>
            </td>
            <td>
                <b>
                    Options for GRPC message size configurable (backport #2805) 2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of pull request #2805

Signed-off-by: Parameswaran Selvam parselva@in.ibm.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 15:23:50 +0000 UTC
    </div>
</div>

