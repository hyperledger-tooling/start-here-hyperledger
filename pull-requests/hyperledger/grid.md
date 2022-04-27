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
                PR <a href="https://github.com/hyperledger/grid/pull/1393" class=".btn">#1393</a>
            </td>
            <td>
                <b>
                    Add `get_failed_batches` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds an operation to get failed batches. This also adds a unit test for the operation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 19:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1392" class=".btn">#1392</a>
            </td>
            <td>
                <b>
                    Upgrade reqwest version to 0.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                0.11 removes an unnecessary trait bound on the post method that we would
otherwise need to implement in the upcoming submitted component.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 16:30:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1391" class=".btn">#1391</a>
            </td>
            <td>
                <b>
                    Add JSON payload infrastructure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds a v2 to the `submit` module which contains structs used to deserialize REST API JSON requests into smart contract actions. Mainly, this adds the infrastructure needed to create Batches based on Grid's smart contracts.

A few specifics for deserializing: 
- Adds interim `DeserializableXPayload` structs for the Pike and Location modules. These structs assist in determining which action is specified in the JSON. 
- Updates the `CreateAgentAction` to be deserialized from the `CreateAgentActionBuilder`. This allows for errors relating to malformed actions to be more specific as to what is wrong with the payload, rather than attempting to deserialize directly into the `Action` itself. This generates the error from the builder's `build` method, rather than the JSON parsing.
- Adds tests for deserializing multiple JSON objects into the `Payload` enum, to verify the process of converting a list of JSON structs into the correct action.
- Adds tests for deserializing Pike actions for the individual actions and the top-level `Payload` object. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 17:23:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1389" class=".btn">#1389</a>
            </td>
            <td>
                <b>
                    Update protoc to 3.20.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 00:59:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1388" class=".btn">#1388</a>
            </td>
            <td>
                <b>
                    Undo batch_tracking migrations key changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                Previously, the migrations for the batch tracking tables were updated
to use a surrogate key composed of the id and service id due to Diesel's
incomplete support for composite foreign keys. This change switches the
primary key back to a composite primary key as well as the related
foreign keys and operations that need to filter based on those foreign
keys will use raw sql via the `sql_query` function.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 18:31:29 +0000 UTC
    </div>
</div>

