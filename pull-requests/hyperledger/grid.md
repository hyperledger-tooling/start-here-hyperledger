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
                PR <a href="https://github.com/hyperledger/grid/pull/976" class=".btn">#976</a>
            </td>
            <td>
                <b>
                    Add update purchase order uid and version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the update payload uid and accepted version number, as well as
tests to verify the translation to and from protobuf.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 20:08:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/975" class=".btn">#975</a>
            </td>
            <td>
                <b>
                    Add `grid po version update` CLI command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds and implements the `grid po version update` CLI command. This
    command is used to update one or more of the editable PO version fields.
    This command handles for adding a new revision if new PO XML is
    submitted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 21:10:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/974" class=".btn">#974</a>
            </td>
            <td>
                <b>
                    Match the db schema to model for Purchase Order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the `PurchaseOrder` database table schema to match
the order the fields exist in the `PurchaseOrderModel` struct.

Previously, this caused an error when diesel attempted to insert the
database model into the table, as the native model does not match the
table's schema.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 16:55:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/973" class=".btn">#973</a>
            </td>
            <td>
                <b>
                    Fix handling of protobuf optional field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes how the `CreateVersionPayload` is being converted by
the purchase order protocol code. Previously, this value was being
pulled from the protobuf, but as it is optional, the value pulled from
the protobuf must first be validated as non-empty. If it is empty, this
field is set to `None`. If not, the `CreateVersionPayload` is converted
into a native struct using it's `from_proto` method.

This fixes an issue where the payload may be set with empty values from
the protobuf.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 20:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/972" class=".btn">#972</a>
            </td>
            <td>
                <b>
                    Re-add `created_at` to PO migrations tables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The created_at field was omitted accidentally when consolidating the
migrations for the purchase_order table. This just adds that back in.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 18:56:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/971" class=".btn">#971</a>
            </td>
            <td>
                <b>
                    Add `workflow_status` to PO version DB structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the workflow_status field to the PO version DB structs.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 15:48:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/970" class=".btn">#970</a>
            </td>
            <td>
                <b>
                    Update built-in workflow display methods to designate version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the built-in purchase order workflows to specify the
version being used for the workflow, and to specify these workflows are
built-in. This changes the formatting of the POWorkflow's type from
`<workflow_type>` to `built-in::<workflow_type>::v1`.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 15:10:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/968" class=".btn">#968</a>
            </td>
            <td>
                <b>
                    Create PO in cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding functionality to create purchase order. Based on the updated RFC,
we need buyer-org and seller-org instead of owning org. Changes are
reflected in the man pages as well as code.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 13:33:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/967" class=".btn">#967</a>
            </td>
            <td>
                <b>
                    Add implementation for "create version" action in po smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR mainly adds an implementation and unit tests for the "create_version" function within the purchase order smart contract's handler.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 22:37:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/966" class=".btn">#966</a>
            </td>
            <td>
                <b>
                    Singularize CLI action modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the names of the CLI action modules to be singular. This
    brings these module names in line with their counterparts in other parts
    of Grid.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 18:26:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/965" class=".btn">#965</a>
            </td>
            <td>
                <b>
                    Update `/purchase-order` to `/purchase_order`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the REST API for purchase orders so that it conforms with a the
lower snake case URL standard.

This PR was created in response to validation problems discovered in https://github.com/hyperledger/grid/pull/959

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 18:18:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/964" class=".btn">#964</a>
            </td>
            <td>
                <b>
                    Require `workflow_status` and `order_xml` args
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes the `workflow_status` and `order_xml` CLI args required for
    the PO version create and update commands. A version/revision doesn't
    provide much utility without these values.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 16:35:55 +0000 UTC
    </div>
</div>

