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

