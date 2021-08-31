---
layout: default
title: firefly-tokens-erc1155
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-tokens-erc1155
---

# firefly-tokens-erc1155 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-tokens-erc1155){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Allow overriding request ID
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
        Created At 2021-08-31 14:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Remove "author" field from token-pool event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Can be merged after https://github.com/hyperledger-labs/firefly/pull/177
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 20:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Add operator to every websocket event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All of the events from this contract include an `operator` indicating the address of the party that performed the operation. This just exposes that upward.

Note: previously the field was remapped to `author` on the pool creation event, but the plan is to standardize on `operator` for this interface. Will remove `author` after firefly core is adjusted to look at the new field.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 18:41:24 +0000 UTC
    </div>
</div>

