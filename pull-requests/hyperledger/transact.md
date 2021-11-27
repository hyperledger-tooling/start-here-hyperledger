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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Drop contexts in serial sched when txns complete
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change drops the appropriate contexts when a transaction is complete or the schedule is canceled.

It updates the current transaction to include its associated context ID so that the context can be dropped on cancellation.  Otherwise, the context would get leaked.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 18:05:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Stabilize transact-cli `workload`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the transact-cli `workload` feature by moving it from
experimental to stable.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 17:55:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    `workload-batch-gen` stabilization updates - fix protobuf use
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization updates for the libtransact `workload-batch-gen` feature, this PR limits the use of Protobuf in the `workload-batch-gen` feature.

- Add two traits `BatchReader` and `TransactionReader`, which provide an API for reading batches and reading transactions from a source.
- Replace the `LengthDelimitedMessageSource` with `ProtobufTransactionReader` and `ProtobufBatchReader` which implement`TransactionReader` and `BatchReader`.
- Update tests to use `ProtobufTransactionReader` and `ProtobufBatchReader`.
- Limit the direct use of protobuf in tests to only the function that writes length delimited protobuf.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 17:49:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Build some crates with target wasm32-unknown-unknown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This catches errors for crates which are usually compiled into smart
contracts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 22:31:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    Update rand dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes rand_hc and updates rand to 0.8.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 20:23:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    Stabilize `family-command-workload`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the `family-command-workload` feature by moving it from
experimental to stable.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 19:56:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    Implement Drop Context
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
        Created At 2021-11-22 19:37:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    `family-command-workload` stabilization updates - API docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add API doc for CommandGeneratingIter, CommandTransactionWorkload, CommandBatchWorkload, and CommandTransactionBuilder 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 18:56:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    Update flexi_logger dependency to v0.20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is intended as a non-functional change the track the latest
dependency.

Adds the "use_chrono_for_offset" feature as required to avoid warnings
from this version of flexi_logger; this is a flexi_logger problem and
can be safely removed when its no longer needed to avoid warnings from
flexi_logger.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 18:05:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Remove experimental database-sqlite feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The database-sqlite feature has been replaced with sqlite support at
a higher level (sqlite+state-merkle-sql features) which allows for
greater efficiencies. So while this feature works, removing it to avoid
duplication of approach.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 17:29:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    `workload` stabilization updates - Add `workload-smallbank` feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a "workload-smallbank" feature to transact-cli and put any code
currently behind the "workload" feature, that is related to smallbank,
behind this new feature.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 16:16:54 +0000 UTC
    </div>
</div>

