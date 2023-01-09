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
                PR <a href="https://github.com/hyperledger/fabric/pull/3904" class=".btn">#3904</a>
            </td>
            <td>
                <b>
                    Add PurgedKeyAuditLogging config option (backport #3901)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3901 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-09 03:06:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3902" class=".btn">#3902</a>
            </td>
            <td>
                <b>
                    Fix approve for my org to not endorse committed transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a chaincode is approved and committed, it means that it has been accepted and added to the network. However, it is still possible to approve the exact chaincode definition with the same sequence after it has been committed. This can lead to confusing behavior because the transaction is endorsed even though it will never be considered valid.

This commit proposes a fix to prevent the endorsement of transactions that attempt to approve already committed chaincode definitions with the same sequence. By failing endorsement of these transactions, we can provide a better experience for end users. In addition, this will help to ensure that the chaincode approval process is more transparent and predictable for all parties involved.

Signed-off-by: Artem Barger <artem@bargr.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 22:33:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3901" class=".btn">#3901</a>
            </td>
            <td>
                <b>
                    Add PurgedKeyAuditLogging config option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add peer config option to log purged private data keys. Useful to audit that private data has been purged from a peer, however some users may want to disable the audit logging to prevent private data keys from appearing in peer logs, while preserving the other pvtdatastorage log messages.

Sample log entry:
```
INFO [pvtdatastorage] process -> Purging private data from private data storage channel=mychannel chaincode=private collection=Org1MSPPrivateCollection key=assetp5 blockNum=12 tranNum=0
INFO [pvtdatastorage] process -> Purging private data from private data storage channel=mychannel chaincode=private collection=Org1MSPPrivateCollection key=assetp5 blockNum=13 tranNum=0
INFO [pvtdatastorage] process -> Purging private data from private data storage channel=mychannel chaincode=private collection=assetCollection key=assetp5 blockNum=12 tranNum=0
INFO [pvtdatastorage] process -> Purging private data from private data storage channel=mychannel chaincode=private collection=assetCollection key=assetp5 blockNum=13 tranNum=0

INFO [pvtdatastorage] deleteDataMarkedForPurge -> Purged private data from private data storage channel=mychannel numKeysPurged=2 numPrivateDataStoreRecordsPurged=4
```

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 22:29:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3900" class=".btn">#3900</a>
            </td>
            <td>
                <b>
                    Endorsement policies doc edited (backport #3890)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3890 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-06 16:51:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3899" class=".btn">#3899</a>
            </td>
            <td>
                <b>
                    Improve gateway retry logic sending to orderers (backport #3897)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3897 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-06 13:08:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3898" class=".btn">#3898</a>
            </td>
            <td>
                <b>
                    Improve gateway retry logic sending to orderers (backport #3897)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3897 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-06 13:04:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3897" class=".btn">#3897</a>
            </td>
            <td>
                <b>
                    Improve gateway retry logic sending to orderers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Status >= 500 errors returned by orderers should retried on other orderers

resolves https://github.com/hyperledger/fabric-gateway/issues/517

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 16:14:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3896" class=".btn">#3896</a>
            </td>
            <td>
                <b>
                    Switch base docker image from golang-alpine to ubuntu:20.04 (backport #3882)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix
- New feature

#### Description

This PR is a back port merge from release-2.5 to mainline of: 

- cherry-pick 114695ab06884242e3cc0d8046137dd2b5b8f36b (#3882)
- cherry-pick 764fd40576598cd8c916c85153e260f5a7257de3  (#3894)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 16:10:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3895" class=".btn">#3895</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove system-channel usage from integration tests: discovery
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

Remove system-channel usage from integration tests: discovery

#### Related issues

Epic: #3511
Issue: #3515

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 15:12:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3894" class=".btn">#3894</a>
            </td>
            <td>
                <b>
                    Remove peer and orderer ENTRYPOINTS as they were breaking the test network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Bug fix

#### Description

In PR #3882 the peer and orderer Dockerfiles introduced an ENTRYPOINT command, breaking the test network's mechanism for launching the containers with the CMD.  This PR reverts the ENTRYPOINT addition for compatibility with the Compose test network.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 14:23:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3892" class=".btn">#3892</a>
            </td>
            <td>
                <b>
                    change order of raft state change notification (backport #3863)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3863 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-04 03:52:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3891" class=".btn">#3891</a>
            </td>
            <td>
                <b>
                    Trim the (optional) semrev leading 'v' when resolving the ccenv image URL (backport #3879)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3879 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-03 14:26:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3890" class=".btn">#3890</a>
            </td>
            <td>
                <b>
                    Endorsement policies doc edited
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - to avoid confusion for any user reading the document.
- to enable direct copying and pasting of the commands

Signed-off-by: Rajat Sharma <Rajat16.Sharma@ril.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->
- Documentation update

#### Description

The default documentation mentioned for [endorsement-policies](https://hyperledger-fabric.readthedocs.io/en/latest/endorsement-policies.html), does not work.

As the samples only use `Org1MSP` or `Org2MSP`, all the examples state `"AND('Org1.peer', 'Org2.peer')"`. These don't work on the test network.

#### Additional details

This is a documentation change that will help a user to use custom endorsements effectively.

#### Related issues
#3884 
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
        Created At 2023-01-03 14:07:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3889" class=".btn">#3889</a>
            </td>
            <td>
                <b>
                    Update jq command in channel config docs (backport #3888)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3888 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-03 11:27:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3888" class=".btn">#3888</a>
            </td>
            <td>
                <b>
                    Update jq command in channel config docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I've found that quotes are needed around the jq target path.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 02:23:34 +0000 UTC
    </div>
</div>

