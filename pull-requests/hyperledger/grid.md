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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/963" class=".btn">#963</a>
            </td>
            <td>
                <b>
                    Add po revision get rest endpoint
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
        Created At 2021-09-30 19:47:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/962" class=".btn">#962</a>
            </td>
            <td>
                <b>
                    Add po revision list rest endpoint
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
        Created At 2021-09-30 19:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/960" class=".btn">#960</a>
            </td>
            <td>
                <b>
                    Add CLI filters to DB ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds filters to some of the PO DB operations that correspond to the filters available in the list/show PO CLI commands.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 19:50:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/959" class=".btn">#959</a>
            </td>
            <td>
                <b>
                    Add OpenAPI validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a GitHub Action to validate the swagger file

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 22:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/958" class=".btn">#958</a>
            </td>
            <td>
                <b>
                    Add purchase order version REST endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a purchase order REST endpoint to retrieve a version provided a
version id and a purchase order.

Related to: https://github.com/hyperledger/grid/issues/867

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 19:53:16 +0000 UTC
    </div>
</div>

