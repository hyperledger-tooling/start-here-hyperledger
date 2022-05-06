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
                PR <a href="https://github.com/hyperledger/grid/pull/1416" class=".btn">#1416</a>
            </td>
            <td>
                <b>
                    Add REST API batch submitter trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This adds a trait for a component resource of the REST API to build and submit batches to an upstream URL. This will be used by endpoints that accept batches, in order to process generic `TransactionPayload`s. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 22:21:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1415" class=".btn">#1415</a>
            </td>
            <td>
                <b>
                    Add `batch_submission` mod and `url_resolver`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Adds the url_resolver submitter subcomponent and the batch_submission
module structure that contains it.

Dependencies: #1413
Resolves: #1414

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 16:19:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1413" class=".btn">#1413</a>
            </td>
            <td>
                <b>
                    Add scope_id and specific batch structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Adds the `ScopeId` trait and the `GlobalScopeId` and `ServiceScopeId` structs. Also adds batch structs specific to the scope IDs and code from Splinter 0.6 for `FullyQualifiedServiceId`.

These will be required in future sub-components.

Resolves: #1406 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 21:50:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1411" class=".btn">#1411</a>
            </td>
            <td>
                <b>
                    Lint dockerfiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 18:42:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1403" class=".btn">#1403</a>
            </td>
            <td>
                <b>
                    Finish implementing boxed batch tracking store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This "finishes" implementation of the batch tracking store by
    implementing the methods for the implementation of the boxed batch
    tracking store. These were previously left as unimplemented for ease of
    updating the operations as they were being implemented.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 18:41:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1402" class=".btn">#1402</a>
            </td>
            <td>
                <b>
                    Update batch tracking store doc comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This updates the doc comments for the batch tracking store methods to be
    up to date with the current implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 18:33:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1401" class=".btn">#1401</a>
            </td>
            <td>
                <b>
                    Make `TrackingBatch` `service_id` an `Option`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This makes the `service_id` field on the `TrackingBatch` struct an
    `Option`. This is in support of work on the batch queuer.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 19:47:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1400" class=".btn">#1400</a>
            </td>
            <td>
                <b>
                    Clean up `BatchTrackingStore` tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This cleans up the batch tracking store tests by putting repetitive,
    shared code into functions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 18:17:33 +0000 UTC
    </div>
</div>

