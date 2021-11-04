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
                PR <a href="https://github.com/hyperledger/transact/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    `family-command` stabilization updates - make handler module private
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `CommandTransactionHandler` is re-exported so the handler module can
be made private.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 17:25:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    `workload-runner` stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a bug where the break statements in the `WorkerBuilder` `build` function didn't properly shutdown the workload. This bug is fixed by switching from using an AtomicBool to a shutdown signaler. Previously an AtomicBool was used to indicate the running state of a workload and a loop was used to keep the workloads running until a sigint was received. With this setup, any break statements in the `WorkerBuilder` `build` function would exit the inner loop and cause the program to hang because the outer loop would not exit until the AtomicBool was changed by the ctrlc handler. Using the shutdown signaler and the `wait_for_shutdown` function allow for the workload to shutdown properly if any errors are encountered. As a result of this change the duration value is passed to the `add_workload` function and used in the `build` function of `WorkerBuilder` to calculate the end time and stop the workload when the end time is reached.

Other stabilization related changes included in this PR:
- Remove an `expect` in the worker thread
- Replace `exit` with `break` in the worker thread
- Add rustdoc comments for `get_batch_status` and `build`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 20:08:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.3.13
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
        Created At 2021-11-02 21:55:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/247" class=".btn">#247</a>
            </td>
            <td>
                <b>
                    Remove openssl dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the openssl dependency.  This library was only used for SHA-512 hashing.  This same functionality can be replaced with the already-included sha2 library.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 20:52:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/246" class=".btn">#246</a>
            </td>
            <td>
                <b>
                    Remove "database-lmdb" from experimental
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the feature "database-lmdb" from the set of experimental features, as it is already stable and included under the default features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 18:02:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/245" class=".btn">#245</a>
            </td>
            <td>
                <b>
                    `Workload` CLI feature stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization updates for the `workload` feature in transact CLI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 18:23:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    Backport 0.3:Delete SqlMerkleState trees
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #236 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 15:39:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    `workload` feature stabilization updates - errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update the methods in the `TransactionWorkload` and `BatchWorkload` traits to use the `InvalidStateError` error type instead of
`WorkloadError`.
- Remove `WorkloadError` from the workload error module.
- Make workload error module private
- `enum_variant_names` clippy lint doesn't allow enum variants to repeat the enum name.
- Put the `BatchReadingError` behind the "workload-batch-gen" feature as this error type is only used by functions behind this feature.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 23:17:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Fix `--duration` help message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the help message for the `--duration` option in the workload CLI
command.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 20:27:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/241" class=".btn">#241</a>
            </td>
            <td>
                <b>
                    Small fixups for `transact playlist` CLI command
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
        Created At 2021-10-29 19:29:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/240" class=".btn">#240</a>
            </td>
            <td>
                <b>
                    Fix outdated rustdoc comment for process_smallbank_playlist
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
        Created At 2021-10-29 16:06:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    `workload` stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization related updates for the workload feature
- Add documentation for the workload module
- Make the source module private and put it behind the "workload-batch-gen" feature because it's only used in the `batch_gen` module which is behind this feature 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 22:56:12 +0000 UTC
    </div>
</div>

