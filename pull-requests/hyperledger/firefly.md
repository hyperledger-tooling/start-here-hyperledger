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
                PR <a href="https://github.com/hyperledger/firefly/pull/587" class=".btn">#587</a>
            </td>
            <td>
                <b>
                    add `fetchreferences` param to events api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `fetchreferences` will add the referred object to the GET /events response

in a chain with #579 

closes #580 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-06 19:32:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    Added version command to Core Binary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Swarnim Pratap Singh <swarnimpratap132@gmail.com>
Fixes #132
It provides a command for listing the firefly build version and creating an internal package for the version so that it was accessible to the versionCmd in the cmd package.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-05 08:10:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    Blockchain metrics for Ethereum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces blockchain metrics for:

- FireFly performing a blockchain transaction with a smart contract method
- FireFly querying the blockchain with a smart contract method
- Events emitted by a smart contract that FireFly is listening for

Each of these has two labels `location` and `methodName` for transactions/queries or `signature` (for events). The `location` is a blockchain specific appropriate string for describing where the event came from. The value of this label is 
 in the format of `"<key1>=<value1>,<key2>=<value2>"`. For Ethereum, it is just `address=<contract_address>`.

Fabric metrics will also be added in a subsequent PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 17:23:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/582" class=".btn">#582</a>
            </td>
            <td>
                <b>
                    Update batch logic to only store+hash the manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolved #506 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 12:58:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/579" class=".btn">#579</a>
            </td>
            <td>
                <b>
                    Enhance subscription filters & event enrichment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - Support for Transaction and BlockchainEvent event filtering
 - Added ws event enrichment for transactions and blockchain events

closes #545 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 21:24:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/578" class=".btn">#578</a>
            </td>
            <td>
                <b>
                    Handle operations with retries in transaction status
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
        Created At 2022-03-03 20:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    Add missing itype column in SQLite migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The testing for #549 focussed on PostgreSQL and one of the updates to the migration got missed in the SQLite one.

Raising and will do a test before looking for a review.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 14:23:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    Update manifest versions
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
        Created At 2022-03-01 21:12:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    Explicitly name all subscriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #554 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 23:33:27 +0000 UTC
    </div>
</div>

