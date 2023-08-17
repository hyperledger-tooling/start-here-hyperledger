---
layout: default
title: harmonia
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/harmonia
---

# harmonia <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/harmonia){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Add Table of Contents to arch doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 13:18:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Add feature to unlock generic Corda asset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implemented the feature to unlock any Corda asset based on a transaction event.
The locked asset can be unlocked by providing:
- a transaction receipt containing the expected event log
- the merkle proof for all the transaction receipts in the block that emitted the event
- the index of the transaction that emitted the event
- the validators signature over the transaction's block header receipts root hash
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 19:14:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Add Architecture level document about C5 to Ethereum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                High level overview of how we're planning on integrating native EVM communication with Corda 5.

Still to come:

- An overview of Corda 5 and Ethereum networks working together (with a picture)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 14:47:54 +0000 UTC
    </div>
</div>

