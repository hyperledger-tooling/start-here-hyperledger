---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1352" class=".btn">#1352</a>
            </td>
            <td>
                <b>
                    Add E2E test for indexing an existing ERC1155
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Requires https://github.com/hyperledger/firefly-tokens-erc1155/pull/129
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 15:58:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1351" class=".btn">#1351</a>
            </td>
            <td>
                <b>
                    Use NetworkName instead of Name for definition topics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1349

Related fix that will also need to be integrated: https://github.com/hyperledger/firefly-common/pull/76
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 15:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    Docs improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding two improvements in docs:

- adding a note for macOS users (port 5000 already in use)
- updating the command to be consistent with previous page (created `dev` stack but next page started `demo`)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 17:27:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1346" class=".btn">#1346</a>
            </td>
            <td>
                <b>
                    Fix uniqueness check in InsertOrGetFFI to match indexes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When guessing the reason for an insert conflict, the query needs to exactly match the configured database indexes. That means that the "name" and "networkName" queries need to both include "version" as well, otherwise we risk grabbing a row that isn't actually a conflict.

Fixes #1347 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 15:58:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1345" class=".btn">#1345</a>
            </td>
            <td>
                <b>
                    FabConnect does not / can not set transactionIndex and eventIndex
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Fabric chaincode events when dispatched to FabConnect by the Fabric SDK do not contain the index within the block:
https://github.com/hyperledger/fabric-sdk-go/blob/7af45cede6afa3939a9574bc9948cca9fb424257/pkg/common/providers/fab/eventservice.go#L43C1-L59

So the only information upon which to build a unique `ProtocolID` for the event is the block number, and the transaction index (noting Hyperledger Fabric has a restriction of one transaction per block).

Under load when multiple events are packed into a single block in Fabric, the FireFly Core code was de-duplicating them as a single event, because they all had the same `ProtocolID`, such as `000000000295/000000/000000` (where the second and third parts are always zeros).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 02:15:36 +0000 UTC
    </div>
</div>

