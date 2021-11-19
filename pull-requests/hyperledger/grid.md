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
                PR <a href="https://github.com/hyperledger/grid/pull/1076" class=".btn">#1076</a>
            </td>
            <td>
                <b>
                    Stabilize SDK's "cylinder-jwt-support" by removing it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change stabilizes the "cylinder-jwt-support" feature by removing it
from the Grid SDK.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 14:34:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1075" class=".btn">#1075</a>
            </td>
            <td>
                <b>
                    Add more `client` feature stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds more stabilization updates for the `client` feature following a second round of reviews.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 22:42:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1072" class=".btn">#1072</a>
            </td>
            <td>
                <b>
                    Update purchase order CLI display
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds workflow type to display fields in CLI when user fetches
information about purchase orders. Renames "workflow type"
to "workflow name" and "workflow status" to "workflow state"
in display formatting. Adds clarity to "Accepted" display field.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 20:32:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1071" class=".btn">#1071</a>
            </td>
            <td>
                <b>
                    Small cli fixes
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
        Created At 2021-11-17 17:00:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1070" class=".btn">#1070</a>
            </td>
            <td>
                <b>
                    Remove `pike-rest-api` feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the `pike-rest-api` feature from the SDK. This
feature is a duplicate of the `rest-api-resources-agent` feature.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 16:20:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1068" class=".btn">#1068</a>
            </td>
            <td>
                <b>
                    Enforce uniqueness for PO alternate IDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the purchase order code to enforce uniqueness for alternate IDs. This adds checks to both the client and PO store to make sure that alternate IDs are only used once per splinter circuit or sawtooth instance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 18:31:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1063" class=".btn">#1063</a>
            </td>
            <td>
                <b>
                    Update "create po" action to handle constraints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the "create po" action in the purchase order smart
contract to concern itself with workflow constraints. This adds further
validation when a user attempts to create a purchase order.

This change also adds a test to validate a purchase order may not be
created if the desired workflow state has a constraint it does not
fulfill.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 14:59:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1062" class=".btn">#1062</a>
            </td>
            <td>
                <b>
                    Add concern for workflow constraints to "create vers" action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds concern for workflow constraints to the "create
version" action of the purchase order smart contract. This also updates
the tests written for this action to re-align with the updated
implementation.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 14:26:50 +0000 UTC
    </div>
</div>

