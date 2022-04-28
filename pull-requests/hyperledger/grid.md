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
                PR <a href="https://github.com/hyperledger/grid/pull/1398" class=".btn">#1398</a>
            </td>
            <td>
                <b>
                    Add `clean_stale_records` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds an operation to clean batch tracking records that were created
    before a specified time. This works by removing batch records with a
    `created_at` value less than the specified timestamp. As the other
    batch tracking tables all use foreign keys derived from the batch_id and
    that use cascading deletes, this will remove the batch record and any
    associated "child" records.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 20:44:28 +0000 UTC
    </div>
</div>

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

