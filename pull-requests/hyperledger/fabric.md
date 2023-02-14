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
                PR <a href="https://github.com/hyperledger/fabric/pull/4015" class=".btn">#4015</a>
            </td>
            <td>
                <b>
                    Close connection to unavailable orderers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, if an orderer goes down, the stale connection to it still remains cached in the gateway registry.  This commit implements similar logic as used by connections to external endorsing peers whereby a stale connection is closed and flushed from the cache allowing future invocations to attempt to reconnect.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 15:56:21 +0000 UTC
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

