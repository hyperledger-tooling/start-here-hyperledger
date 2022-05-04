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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1399" class=".btn">#1399</a>
            </td>
            <td>
                <b>
                    Add support for `data_change_id`s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds support for looking up batches by `data_change_id` to batch
    tracking operations that take a batch ID as an argument.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 19:41:38 +0000 UTC
    </div>
</div>

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

