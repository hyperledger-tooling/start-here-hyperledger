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
                PR <a href="https://github.com/hyperledger/fabric/pull/3285" class=".btn">#3285</a>
            </td>
            <td>
                <b>
                    Ledgerutil identifytxs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
- The Identify Transactions tool (identifytxs) is a new addition to the Fabric ledger utilities that adds another layer of troubleshooting to the first Fabric ledger utilities tool, Compare Snapshots. After a user has obtained the list of different records between two snapshots using Compare Snapshots, the user can then pass this output to the Identify Transactions tool to obtain a list of relevant transactions that could potentially be the cause of the initial ledger divergence.
- This PR builds on top of a previous commit by @shimos and extends their work into a complete Fabric ledger utilities tool.

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

- #2788
- #2979 
- #2980 

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
        Created At 2022-03-15 01:13:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3284" class=".btn">#3284</a>
            </td>
            <td>
                <b>
                    Ignore channel double creation during replication.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #2931

Signed-off-by: Jay Guo <guojiannan1101@gmail.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix


#### Description

see details in issue discussion

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
        Created At 2022-03-14 06:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3283" class=".btn">#3283</a>
            </td>
            <td>
                <b>
                    Refactor of ChaincodeEvents service implementation to support resume
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables the client to (optionally) specify a "previously seen" transaction ID in addition to a start block number when requesting chaincode events, which causes chaincode events up to that transaction ID (inclusive) to be ignored and not returned to the client. This supports resume of chaincode event listening on client reconnect without duplicating or missing any events.

Protobuf message changes are required to fully implement and enable this behaviour, but this refactor puts in place the server-side changes and unit tests (albeit commented out in places).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 13:09:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3282" class=".btn">#3282</a>
            </td>
            <td>
                <b>
                    Update ordererchecklist.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                change default path for snapshot in description from /var/hyperledger/production/orderer/etcdraft/wal to /var/hyperledger/production/orderer/etcdraft/snapshot



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 05:51:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3281" class=".btn">#3281</a>
            </td>
            <td>
                <b>
                    Documentation for peer.gossip.externalEndpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">doc-merge</span>
            </td>
            <td>
                Fix the reference to EXTERNAL_ENDPOINT and clarify externalEndpoint role in service discovery.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-11 13:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3273" class=".btn">#3273</a>
            </td>
            <td>
                <b>
                    doc: remove duplicate text on network section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: zufardhiyaulhaq <zufardhiyaulhaq@gmail.com>

remove duplicate text on the network section documentation

#### Type of change

- Documentation update

#### Description

remove duplicate text on the network section documentation

#### Additional details

N/A

#### Related issues

N/A


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 17:00:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3272" class=".btn">#3272</a>
            </td>
            <td>
                <b>
                    Add in the CCAAS builders to the tgz package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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
        Created At 2022-03-09 09:29:50 +0000 UTC
    </div>
</div>

