---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/903" class=".btn">#903</a>
            </td>
            <td>
                <b>
                    Implement some methods for Purchase Order state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds implementations for a few methods on the Purchase Order state that are used by the smart contract actions. This pr adds implementations for the methods `get_purchase_order`, `set_purchase_order`, `get_agent`, and `get_organization`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 19:10:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/902" class=".btn">#902</a>
            </td>
            <td>
                <b>
                    Add workflow-aware has_permission check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a new version of the has_permission check that is used in
other smart contracts. This check is workflow-aware by checking against
workflow permissions and transition permissions. This is used in the
same way as the original has_permission check. Agents will need to have
Pike roles with permissions that map to the names of Workflow permission
aliases for the given workflow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 17:58:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/901" class=".btn">#901</a>
            </td>
            <td>
                <b>
                    Add initial implementation of the "create purchase order" action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes a few updates to the purchase order protos and corresponding protocol code. This also adds an initial implementation of the "create purchase order" action for the Purchase Order smart contract's transaction handler.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 21:37:49 +0000 UTC
    </div>
</div>

