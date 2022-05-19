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
                PR <a href="https://github.com/hyperledger/fabric/pull/3431" class=".btn">#3431</a>
            </td>
            <td>
                <b>
                    Improve response mismatch logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit addresses some comments (https://github.com/hyperledger/fabric/pull/3420#pullrequestreview-978439334) made on the original PR for this feature as follows:
- The mismatch details are logged as warnings through a new logger “gateway.responsechecker”.  This is enabled by default but can be disabled by setting the log level to “error” for this logger.
- Each log message contains the address/mspid of the initial endorser and ’this’ endorser.  The ‘expected’ &’ actual’ values have been renamed ‘initial’ and ‘this’ accordingly.
- Spaces in the insert names have been replaced by hyphens for improved readability since the logger removes the spaces in the output.
- The base64 encoded protobuf responses have been removed from the log since they are now redundant.

Log entries look like this:
```
[e][Org1.peer0] 2022-05-19 16:21:41.695 BST 00a2 WARN [gateway] processEndorsement -> ProposalResponsePayloads do not match. See [gateway.responsechecker] log warnings for details.
[e][Org1.peer0] 2022-05-19 16:21:41.695 BST 00a3 WARN [gateway.responsechecker] processEndorsement -> Compared to the initial endorser's response, the following log entries detail the differences in this endorser's response. initial-endorser="127.0.0.1:22005 (Org1MSP)" this-endorser="127.0.0.1:22010 (Org2MSP)"
[e][Org1.peer0] 2022-05-19 16:21:41.695 BST 00a4 WARN [gateway.responsechecker] processEndorsement -> Proposal response mismatch: initial-endorser="127.0.0.1:22005 (Org1MSP)" this-endorser="127.0.0.1:22010 (Org2MSP)" type="write value mismatch" namespace=pvtmarblescc key=key1 initial-value=Org1MSP this-value=Org2MSP
[e][Org1.peer0] 2022-05-19 16:21:41.695 BST 00a5 WARN [gateway.responsechecker] processEndorsement -> Proposal response mismatch: initial-endorser="127.0.0.1:22005 (Org1MSP)" this-endorser="127.0.0.1:22010 (Org2MSP)" type="write metadata mismatch (SBE policy)" namespace=pvtmarblescc key=key1 name=VALIDATION_PARAMETER initial-value="rule:<n_out_of:<n:1 rules:<signed_by:0 > > > identities:<principal:\"\\n\\007Org1MSP\\020\\003\" > " this-value="rule:<n_out_of:<n:1 rules:<signed_by:0 > > > identities:<principal:\"\\n\\007Org2MSP\\020\\003\" > "
[e][Org1.peer0] 2022-05-19 16:21:41.695 BST 00a6 WARN [gateway.responsechecker] processEndorsement -> Proposal response mismatch: initial-endorser="127.0.0.1:22005 (Org1MSP)" this-endorser="127.0.0.1:22010 (Org2MSP)" type="private collection hash mismatch" namespace=pvtmarblescc collection=collectionMarbles initial-hash=efb38ca7ac94ce312d186cfb6da62b67f06fe889099b421fde3a4a7f5dec06fe this-hash=f713a7a5e5f0412c226af7bfc2a3eb0d0c7a3099f09a7a45e99d3424c37d9234
[e][Org1.peer0] 2022-05-19 16:21:41.695 BST 00a7 WARN [gateway.responsechecker] processEndorsement -> Proposal response mismatch: initial-endorser="127.0.0.1:22005 (Org1MSP)" this-endorser="127.0.0.1:22010 (Org2MSP)" type="chaincode event mismatch" initial-event="chaincodeId: pvtmarblescc, name: my-event, value: Org1MSP" this-event="chaincodeId: pvtmarblescc, name: my-event, value: Org2MSP"
[e][Org1.peer0] 2022-05-19 16:21:41.695 BST 00a8 WARN [gateway.responsechecker] processEndorsement -> Proposal response mismatch: initial-endorser="127.0.0.1:22005 (Org1MSP)" this-endorser="127.0.0.1:22010 (Org2MSP)" type="chaincode response mismatch" initial-response="status: 200, message: , payload: Org1MSP" this-response="status: 200, message: , payload: Org2MSP"

```


Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 16:30:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3430" class=".btn">#3430</a>
            </td>
            <td>
                <b>
                    Remove redundant type definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The code that used this was rewritten in a previous commit.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 14:07:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3429" class=".btn">#3429</a>
            </td>
            <td>
                <b>
                    Fix some errors in the tutorial
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

- Documentation update

#### Description

This is a backport of the commit 318510f80a to release-2.2.

Signed-off-by: Satoshi Ito <satoshi.ito.tf@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 04:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3428" class=".btn">#3428</a>
            </td>
            <td>
                <b>
                    Update doc CouchDB links to 3.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Address comments from release-2.4 PR.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 16:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3427" class=".btn">#3427</a>
            </td>
            <td>
                <b>
                    new caas page (backport #3329)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3329 done by [Mergify](https://mergify.com).


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
        Created At 2022-05-17 18:39:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3426" class=".btn">#3426</a>
            </td>
            <td>
                <b>
                    New Block Attestation Orderer GRPC service
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
New RPC service for block attestation is added. It will be used by BFT block replication

#### Related issues
#3413 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 10:20:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3424" class=".btn">#3424</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix code issues from the updated staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 20:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3423" class=".btn">#3423</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update staticcheck to a version that works with Go 1.18.
Fix code issues with the new staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 19:45:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3420" class=".btn">#3420</a>
            </td>
            <td>
                <b>
                    Log proposal response differences
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the gateway, if proposal responses from different endorsing peers don’t match, then it’s very difficult for the end user to diagnose why.  This commit adds extra logging to help identify the cause of the mismatch.

If the log level is set to ‘debug’ for the ‘gateway’, then the proposal response payloads are unmarshalled and analysed to log specific differences between individual key/values in the read/write sets, SBE policy write differences, event differences and chaincode response differences.  For private collections, only the hashes are logged if they are different.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 12:06:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3418" class=".btn">#3418</a>
            </td>
            <td>
                <b>
                    Fix mistake change 'curl' to 'git'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-14 14:23:58 +0000 UTC
    </div>
</div>

