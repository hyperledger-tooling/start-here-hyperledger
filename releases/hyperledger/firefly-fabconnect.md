---
layout: default
title: firefly-fabconnect
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.9.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.9.12
                </span>
            </td>
            <td>
                ## What's Changed
- Added new endpoint for querying block using transaction ID: `GET /blockByTxId/:txId`
- Enhanced chaincode query endpoint to support single-peer queries and "strongread" with the endpoint: `GET /query`
- Added support to use block hash to query for a block, in addition to block number with the endpoint `GET /blocks/:blockNumberOrHash`
- Fill in the `chaincodeId` and `transactionId` fields in event payload even if the transaction did not publish any events

**Full Changelog**: https://github.com/hyperledger/firefly-fabconnect/compare/v0.9.11...v0.9.12
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.12" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-11 17:58:57 +0000 UTC
    </span>
</div>

