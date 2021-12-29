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
                PR <a href="https://github.com/hyperledger/grid/pull/1210" class=".btn">#1210</a>
            </td>
            <td>
                <b>
                    Update `po update` command to allow simultaneous version updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds options and flags to enable simultaneous changes to purchase orders and
versions in situations where step-wise updates would lead to invalid states.

Users may only update the components of the version workflow state that must
be changed to avoid invalid states when updating purchase orders.

Resolves: #1202, #1183

Requires: #1199
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 20:10:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1207" class=".btn">#1207</a>
            </td>
            <td>
                <b>
                    update create po handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the structure and layout of the purchase order smart contract's create po action. This also updates the tests to be valid with the additional validation checks happening in the smart contract. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 16:31:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1206" class=".btn">#1206</a>
            </td>
            <td>
                <b>
                    Enable missing imports for purchase order feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several imports that should be enabled for the purchase order feature
were disabled. This change enables them.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 15:08:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1205" class=".btn">#1205</a>
            </td>
            <td>
                <b>
                    Move PO CLI public modules before function definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 14:53:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1204" class=".btn">#1204</a>
            </td>
            <td>
                <b>
                    Update copyright to 2021 for all that were 2019 for PO CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 14:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1203" class=".btn">#1203</a>
            </td>
            <td>
                <b>
                    Add `workflow_name` arg to `grid po create`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a required arg to specify the po workflow when
creating a PO. Previously, all POs defaulted to the
collaborative workflow. Uses workflow-name instead
of workflow-type to be consistent with the CLI
display.

Resolves: #1201

Requires: https://github.com/hyperledger/grid/pull/1199

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 22:37:44 +0000 UTC
    </div>
</div>

