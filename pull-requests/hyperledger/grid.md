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
                PR <a href="https://github.com/hyperledger/grid/pull/998" class=".btn">#998</a>
            </td>
            <td>
                <b>
                    Make workflow status required for `po create`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PO create command will panic if no workflow status is passed, and
the CreatePurchaseOrderPayloadBuilder requires it to function. This
change makes clap force the user to pass a workflow status.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 16:35:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/996" class=".btn">#996</a>
            </td>
            <td>
                <b>
                    Add alternate_id support to PO state proto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds support for alternate IDs to the Purchase Order state proto.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 20:33:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/995" class=".btn">#995</a>
            </td>
            <td>
                <b>
                    Add `alternate_id` support to `grid po create` CLI command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds support for adding alternate IDs to the `grid po create`
    command. Previously, this was omitted due to lack of support in the
    store and protocol code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 19:56:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/994" class=".btn">#994</a>
            </td>
            <td>
                <b>
                    Base grid-cli on focal instead of sabre-cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously we had a need for sabre cli alongside the grid cli but this is no
longer the case.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 15:58:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/990" class=".btn">#990</a>
            </td>
            <td>
                <b>
                    Implement list/show version fns for reqwest client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements the functions to list and show PO versions in the reqwest client.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 20:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/989" class=".btn">#989</a>
            </td>
            <td>
                <b>
                    Implement list/show revisions in the reqwest client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements the `list_purchase_order_revisions` and `get_purchase_order_revision` functions in the reqwest client.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 17:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/988" class=".btn">#988</a>
            </td>
            <td>
                <b>
                    Update purchase order to use actix path tuples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Actix requires that all URL params are defined in a single path tuple.
This change allows actix to correctly process requests to specific
purchase order endpoints.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 15:06:18 +0000 UTC
    </div>
</div>

