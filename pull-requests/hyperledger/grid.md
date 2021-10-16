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
                PR <a href="https://github.com/hyperledger/grid/pull/984" class=".btn">#984</a>
            </td>
            <td>
                <b>
                    Add constraints to built-in workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously, the built-in workflows defined for the Purchase Order smart contract did not define any constraints between workflow states. This pr adds an enum (to make these variants easily accessible to the smart contract which will need to now ask the workflow state for any constraints it may have to verify the po state) for the possible workflow constraints.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 18:07:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/983" class=".btn">#983</a>
            </td>
            <td>
                <b>
                    Add SplinterProtocolVersion to app auth handler registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will enable getting the correctly formatted version of
AdminEvents from 0.5 splinter nodes and should be ignored
from 0.4 splinter nodes.

Required for backward compatibility.

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 15:46:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/982" class=".btn">#982</a>
            </td>
            <td>
                <b>
                    Wrap ffi types in safe structs, with constructors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the ffi code used by the `data_validation` module to
better encapsulate the pointers being produced by the unsafe functions.

This adds checks that the pointers being returned are not null and adds
more error handling when a pointer is null.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 14:33:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/981" class=".btn">#981</a>
            </td>
            <td>
                <b>
                    Update `From` impls and migration data to match expected db schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes two bugs present when attempting to insert a po record into the db. 

* Fixes the data type of the `id` field in the postgres migration data. Previously, this was `INTEGER` rather than `BIGSERIAL`, which caused the database to not automatically increment this field when inserting a new record into the db and would error because of this null value. 
* Fixes the migration data and `From` implementations of the `purchase_order` db table to ensure the `workflow` status field is where it is expected as defined by the purchase order schema. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 14:28:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/980" class=".btn">#980</a>
            </td>
            <td>
                <b>
                    Implement Update PO CLI action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements the `grid po update` CLI command. This follows the patterns established by other commands. Additionally, this update required that a lot of the gaps in PO, especially surrounding alternate IDs, be filled in.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 19:14:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/979" class=".btn">#979</a>
            </td>
            <td>
                <b>
                    Add update purchase order action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds an implementation of the update purchase order action
to Grid contracts.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 17:58:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/978" class=".btn">#978</a>
            </td>
            <td>
                <b>
                    Update "create po" smart contract action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the "create po" action implementation to handle the `workflow_status` now present in the `CreatePurchaseOrderPayload` and the `CreateVersionPayload`. 

Previously, this action assumed the intended `workflow` status based on the state of the payload. Now, the purchase order is created with the intended `workflow_status` in mind and this transition is validated rather than what the action assumes the desired workflow state is. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 15:52:09 +0000 UTC
    </div>
</div>

