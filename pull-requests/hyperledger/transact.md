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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.3.14
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Schwarz <pschwarz@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 22:42:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    Back-port 0-3: Add list trees to MerkleRadixStore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                back-port of #270 into the 0-3 branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 16:44:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    `family-smallbank-workload` stabilization updates - add smallbank protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization updates for `family-smallbank-workload`

- Add smallbank protocol
- Refactor code to use protocol instead of protobuf
- Remove panics from `SmallbankGeneratingIter`
- Remove pub from `bytes_to_hex_str`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 00:12:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    Rename GHA workflow files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If workflows share the name filename as an existing workflow in the main
branch, github will execute the workflow from main instead of the branch
appropriate instance.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 21:32:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    Package man pages
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
        Created At 2021-11-18 21:12:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    Add list trees to MerkleRadixStore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `list_trees` method to the `MerkleRadixStore` and provides the necessary operations to enable the new method. 

As this is not a method directly associated with `SqlMerkleState`, this PR also makes the store module and the store itself public, such that this method can be used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 21:00:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    `command` transact-cli stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a comment to command get-state man page to specify nothing is returned.
- Fix the example commands in each of the command man pages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 23:31:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    `playlist` transact-cli stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization updates for the `playlist` feature in transact-cli
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 23:04:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    Add missing arguments to rust doc for WorkloadRunner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 18:39:02 +0000 UTC
    </div>
</div>

