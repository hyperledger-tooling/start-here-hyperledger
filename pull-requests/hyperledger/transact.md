---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/295" class=".btn">#295</a>
            </td>
            <td>
                <b>
                    Release notes for v0.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also updates the main branches release notes to include all of the 0.3.x releases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 21:37:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Correct tests after txn id type change
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes batch_gen tests to account for the change in the transaction_ids type in the BatchHeader struct.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 18:10:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/293" class=".btn">#293</a>
            </td>
            <td>
                <b>
                    Stabilize `workload-batch-gen` in libtransact
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the `workload-batch-gen` feature by moving it from
experimental to stable.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 17:50:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/292" class=".btn">#292</a>
            </td>
            <td>
                <b>
                    Remove unused `source.rs` file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove the Remove unused `source.rs` file from libtransact
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 17:02:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    Change batch header txn ids to String
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changes the batch header's transaction_ids fields from bytes to Strings.  This makes the header signature reference consistent with all other usages of the value "types".

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 16:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    Stabilize `workload-runner` in libtransact
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the `workload-runner` feature in libtransact by moving it
from experimental to stable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 21:10:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/289" class=".btn">#289</a>
            </td>
            <td>
                <b>
                    Remove `workload-batch-gen` from `workload-runner`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update `workload-runner` to no longer pull in the `workload-batch-gen` feature because `workload-runner` does not use any code in this feature.
- Update the playlist feature in transact-cli to pull in `transact/workload-batch-gen`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 21:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/288" class=".btn">#288</a>
            </td>
            <td>
                <b>
                    Move `command` and `workload` features to default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move `command` and `workload` features to default 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 19:27:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    Stabilize transact-cli `command`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the transact-cli `command` feature by moving it from
experimental to stable.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 18:54:00 +0000 UTC
    </div>
</div>

