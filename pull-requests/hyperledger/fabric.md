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
                PR <a href="https://github.com/hyperledger/fabric/pull/3446" class=".btn">#3446</a>
            </td>
            <td>
                <b>
                    Use any peer to evaluate system chaincode transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                System chaincodes are not included in the installed chaincodes returned by service discovery. The Gateway service was relying on discovery results to find peers on which to evaluate transactions and so failed to evaluate system chaincode transaction functions. Now the Gateway service uses any network peer to evaluate transactions invoked on known built-in system chaincodes.

Also added a system test to confirm that the Gateway service can endorse system chaincode transaction functions.

Closes hyperledger/fabric-gateway#434
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 16:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3445" class=".btn">#3445</a>
            </td>
            <td>
                <b>
                    Improved gateway error for transient data failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When transient data is passed to the gateway in a transaction submit, the gateway is more cautious about which orgs it will select to endorse.  It alters the ChaincodeInterest to only allow orgs that are in the distribution policy for the PDCs written to by the chaincode.
This commit doesn’t change the behaviour, but gives a more helpful error message if this layer of protection caused the submit to fail due to the lack of endorsing orgs.
This will help to diagnose issues such as #3328 which took a long time to resolve because of the generic error message.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 14:44:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3442" class=".btn">#3442</a>
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
                #### Type of change

- Documentation update

#### Description

This patch is a solution for errors that occur in the tutorial "Using CouchDB".
First, we added environment variables as in the other tutorials.
Second, we added information to authenticate when using CouchDB.

Signed-off-by: Satoshi Ito <satoshi.ito.tf@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 00:40:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3441" class=".btn">#3441</a>
            </td>
            <td>
                <b>
                    Improve response mismatch logging (backport #3431)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3431 done by [Mergify](https://mergify.com).


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
        Created At 2022-05-23 12:18:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3440" class=".btn">#3440</a>
            </td>
            <td>
                <b>
                    Log proposal response differences (backport #3420)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of #3420

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 09:29:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3439" class=".btn">#3439</a>
            </td>
            <td>
                <b>
                    Delete historical versions of private data marked for purging (#3024)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature

#### Description
This PR includes
  - Code for processing the purge marker in the background that deletes
  the historical versions of the private data and corresponding
  hashed-indexed-keys that qualifies for deletion
  - Modifies the transaction number match in the previously committed
   code for filtering the 'to be purged' data so as to have the same
   behavior as for the actually purged data.

#### Related issues
Closes #3024 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 03:51:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3437" class=".btn">#3437</a>
            </td>
            <td>
                <b>
                    bump Go to 1.18.2 (release-2.2) 3 of 3
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
        Created At 2022-05-20 21:38:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3436" class=".btn">#3436</a>
            </td>
            <td>
                <b>
                    bump golang.org/x/crypto and golang.org/x/tools (release-2.2) 2 of 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump dependencies in preparation for Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 21:25:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3435" class=".btn">#3435</a>
            </td>
            <td>
                <b>
                    bump go-dockerclient (release-2.2) 1 of 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #2338 in preparation of Go 1.18 update.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 20:56:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3433" class=".btn">#3433</a>
            </td>
            <td>
                <b>
                    [Doc] Remove text for a broken link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

Remove text and broken link


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 08:16:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3432" class=".btn">#3432</a>
            </td>
            <td>
                <b>
                    Remove duplicated line
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
        Created At 2022-05-20 06:50:30 +0000 UTC
    </div>
</div>

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

