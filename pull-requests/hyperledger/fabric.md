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
                PR <a href="https://github.com/hyperledger/fabric/pull/4011" class=".btn">#4011</a>
            </td>
            <td>
                <b>
                    Orderer v3: fix IsChannelMember to match public keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Bug fix
- Improvement (improvement to code, performance, etc)
- 
#### Description

Orderer v3: fix IsChannelMember to match public keys

- Remove system channel usage from:  `integration/raft/cft_test.go` use-case: "disregards certificate renewal if only the validity period changed"
- Fix a bug in IsChannelMember  that manifested in that test
- Addresses the bug reported in issue #3998

#### Related issues

Addresses: #3998 
Parent issue: #3515 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 12:33:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4010" class=".btn">#4010</a>
            </td>
            <td>
                <b>
                    Return orderer error text to client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a call from the gateway to an orderer node returns an error in the BroadcastResponse message, then it is appended to the details field of the rpc error that gets returned to the client application.  However, the Info field of that message is not getting passed on, so the client could be lacking valuable information on the underlying cause of the error.  This commit fixes that.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 09:54:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4009" class=".btn">#4009</a>
            </td>
            <td>
                <b>
                    Add Performance Considerations to docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

A Section in the fabric documentation to discuss Performance


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-08 14:02:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4006" class=".btn">#4006</a>
            </td>
            <td>
                <b>
                    Address private data purge integration test comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Address comments from https://github.com/hyperledger/fabric/pull/3991.

Namely, speed up reconciliation test by looking for reconcilliation message rather than sleeping for 30s.
Also change default reconcilliation from 10s to 5s to speed up tests.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 20:29:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4003" class=".btn">#4003</a>
            </td>
            <td>
                <b>
                    Update Deployment Documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Aim is to add in more information about deployments.To do this the section on production deployments has been refactored to make it easier to add information.

Not all the additional Information has been added in this commit.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>

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
        Created At 2023-02-07 15:16:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4002" class=".btn">#4002</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: raft no.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Orderer v3: Remove system channel usage from integration tests: raft no.3

#### Additional details

A bug in one of the use cases will be fixed in a future commit, see #3998 

#### Related issues

Issue: #3515 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 14:56:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4001" class=".btn">#4001</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc to v1.1.4 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves dependency vulnerability mentioned in #3989.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 14:29:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4000" class=".btn">#4000</a>
            </td>
            <td>
                <b>
                    Gateway registry should provide cluster size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When submitting a transaction to BFT orderers, the gateway needs to know the number of consenters in the channel config as well as the array of connected orderers.  The quorum size size is calculated from the former which might be larger than the size of the latter.  These two values should be returned by the same registry lookup to ensure they are not out of sync.

Resolves the PR comment for the previous commit:
https://github.com/hyperledger/fabric/pull/3975#discussion_r1098447996

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 14:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3999" class=".btn">#3999</a>
            </td>
            <td>
                <b>
                    Fix ledger integration test flake (backport #3995)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3995 done by [Mergify](https://mergify.com).


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
        Created At 2023-02-07 13:16:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3997" class=".btn">#3997</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.4.3 to 1.5.16 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bumps github.com/containerd/containerd from 1.4.3 to 1.5.16.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 20:12:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3996" class=".btn">#3996</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc to v1.1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves dependency vulnerability mentioned in #3989.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 18:55:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3995" class=".btn">#3995</a>
            </td>
            <td>
                <b>
                    Fix ledger integration test flake
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Need to ensure new peer has joined gossip network before invoking chaincode.

Resolves #3946.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 18:16:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3994" class=".btn">#3994</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: e2e again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: e2e again


#### Related issues

Epic: https://github.com/hyperledger/fabric/issues/3511
Issue: https://github.com/hyperledger/fabric/issues/3515

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 08:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3993" class=".btn">#3993</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: raft no.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: Ie801bbf66b5ae320fbb1f8a099f1cc4b2070ec94

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: raft no.2

#### Related issues
Epic: https://github.com/hyperledger/fabric/issues/3511
Issue: https://github.com/hyperledger/fabric/issues/3515

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 16:42:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3991" class=".btn">#3991</a>
            </td>
            <td>
                <b>
                    Expedite purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Combine purge private data tests into a single 'It' to improve speed (18 minutes to 5 minutes).
This will remove the excessive network teardowns, network builds, and chaincode deployments.
Also remove unneccessary delays and redundant ledger entries.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-04 21:15:17 +0000 UTC
    </div>
</div>

