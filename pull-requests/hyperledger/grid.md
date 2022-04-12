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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1378" class=".btn">#1378</a>
            </td>
            <td>
                <b>
                    Switch Publish Release GHA to run on self-hosted runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 16:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1377" class=".btn">#1377</a>
            </td>
            <td>
                <b>
                    Bump grid-dev version to v10 to differentiate it from 0-3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 18:30:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1376" class=".btn">#1376</a>
            </td>
            <td>
                <b>
                    Backport 0-3: Fix over-eager clone
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-3</span>
            </td>
            <td>
                This change fixes a clippy warning from Rust 1.60. For more information
on this clippy lint, see:
https://rust-lang.github.io/rust-clippy/master/index.html#iter_overeager_cloned

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 17:17:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1375" class=".btn">#1375</a>
            </td>
            <td>
                <b>
                    Fix over-eager clone
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Backport-0-3</span><span class="chip">main</span>
            </td>
            <td>
                This change fixes a clippy warning from Rust 1.60. For more information
on this clippy lint, see:
https://rust-lang.github.io/rust-clippy/master/index.html#iter_overeager_cloned

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 14:54:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1374" class=".btn">#1374</a>
            </td>
            <td>
                <b>
                    Add `change_batch_to_submitted` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This implements the `change_batch_to_submitted` DB operation for the
    Batch Tracking store. This includes a couple unit tests for the
    operation as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 20:57:54 +0000 UTC
    </div>
</div>

