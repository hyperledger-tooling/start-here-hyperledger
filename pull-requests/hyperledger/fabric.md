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
                PR <a href="https://github.com/hyperledger/fabric/pull/3292" class=".btn">#3292</a>
            </td>
            <td>
                <b>
                    Change membership documentation about public keys
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
> a mechanism is required to enable that proof which is where the MSP comes in

Identity can be proven just by signing the transaction and verifying with the public key on the certificate, proving identity is not where the MSP comes in, this is more related to how CAs issue the key-pair.

> The private key is used to produce a signature on a transaction that only the corresponding public key, that is part of an MSP, can match.

The sentence does not say anything about whether this public key matches invalid signatures, it only says that given that particular signature, only that particular public key can match. It should go along the lines of "only a valid signature will work". The sentence has been removed as I have adapted the paragraph.

I do not have experience with Fabric; these changes are based off my reading of the documentation. Am I right to assume that the member's public keys do not need to be added to the organization's MSP in the current version? Please correct me if I am wrong. Thank you.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-19 13:58:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3289" class=".btn">#3289</a>
            </td>
            <td>
                <b>
                    Locate correct block number for transaction ID in ChaincodeEvents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the request contains an `after_transaction_id`, start reading from the block containing that transaction ID and ignore any specified start block. If the specified transaction has not been committed in a block, fall back to any specified start block or next committed block.

Enhancement requested in review of PR #3283
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 14:33:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3288" class=".btn">#3288</a>
            </td>
            <td>
                <b>
                    Ignore channel double creation during replication. (backport #3284)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3284 done by [Mergify](https://mergify.com).


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
        Created At 2022-03-16 04:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3287" class=".btn">#3287</a>
            </td>
            <td>
                <b>
                    Ignore channel double creation during replication. (backport #3284)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3284 done by [Mergify](https://mergify.com).


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
        Created At 2022-03-16 04:58:50 +0000 UTC
    </div>
</div>

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
                Enables the client to (optionally) specify an AfterTransactionId property in addition to a start block number when requesting chaincode events, which causes chaincode events up to that transaction ID (inclusive) to be ignored and not returned to the client. This supports resume of chaincode event listening on client reconnect without duplicating or missing any events.
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

