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
                PR <a href="https://github.com/hyperledger/fabric/pull/3911" class=".btn">#3911</a>
            </td>
            <td>
                <b>
                    [WIP] Check PurgedKeyAuditLogging messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 18:08:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3910" class=".btn">#3910</a>
            </td>
            <td>
                <b>
                    Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Include multiple purge transactions in a single block

Also removes placeholder for seperate test to check data is actually removed from the peer since there is no api available to confirm that- see issue #3844

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 17:08:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3909" class=".btn">#3909</a>
            </td>
            <td>
                <b>
                    Rename ThreeOrgRaft nwo standard networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The name has changed in the main branch as a result of hyperledger#3643 and hyperledger#3853, and this rename should make it easier to backport PRs with mergify

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 11:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3907" class=".btn">#3907</a>
            </td>
            <td>
                <b>
                    Fail-fast fetching potentially purged data during block commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

This PR avoids keep trying behavior for fetching private data during block commit, in a situation where the hashes may not match because the private data may potentially have been purged. Instead, such data is treated as an eligible missing data that the peer would try later in the background reconciliation process.

#### Type of change
- New feature

#### Related issues
[Issue #3858](https://github.com/hyperledger/fabric/issues/3858)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 23:56:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3906" class=".btn">#3906</a>
            </td>
            <td>
                <b>
                    [WIP] Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add scenario1 from #3858

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 17:40:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3905" class=".btn">#3905</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: configtx
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

Remove system channel usage from integration tests: configtx

#### Related issues

Epic:#3511
Issue: #3515


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 15:13:35 +0000 UTC
    </div>
</div>

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

