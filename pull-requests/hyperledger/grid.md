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
                PR <a href="https://github.com/hyperledger/grid/pull/1383" class=".btn">#1383</a>
            </td>
            <td>
                <b>
                    WIP: Add `list_batches_by_status` operation
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
        Created At 2022-04-13 16:57:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1381" class=".btn">#1381</a>
            </td>
            <td>
                <b>
                    Add `get_unsubmitted_batches` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This implements the `get_unsubmitted_batches()` operation for the
    batch tracking store. This operation gets all batches that have not yet
    been sumbitted. This is used by the batch queuer.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 19:57:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1380" class=".btn">#1380</a>
            </td>
            <td>
                <b>
                    Update batch tracking migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This updates the database schema for the batch tracking tables by
adding batch/transaction ID columns. These columns are intended to be
the primary keys for a table and consist of a hash of the batch/txn
header and the service ID. Columns for the service ID and batch/txn
headers are also included for deserialization sake. This is a necessary
change because diesel does not fully support composite keys.
Specifically, it does not implement the `BelongsToDsl` trait for
composite keys and they do not intend to implement this functionality,
as stated in https://github.com/diesel-rs/diesel/issues/1413.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 21:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1379" class=".btn">#1379</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-3: Publish multi-arch Docker images
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
        Created At 2022-04-08 19:04:56 +0000 UTC
    </div>
</div>

