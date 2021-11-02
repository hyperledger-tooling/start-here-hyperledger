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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    Stabilize protocol-sabre by moving to stable
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
        Created At 2021-10-28 15:53:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    `workload-runner` stabilization changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - make `DEFAULT_LOG_TIME_SECS` const private
- make `runner` module private
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 21:10:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Delete SqlMerkleState trees
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
        Created At 2021-10-27 16:18:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    Drop experimental redis support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature is no longer of interest as it does not provide enough of the transactional guarantees required for its usage with merkle state.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 15:28:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Smallbank updates for stabilization
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
        Created At 2021-10-27 15:05:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/233" class=".btn">#233</a>
            </td>
            <td>
                <b>
                    Replace expect with invalid transaction in command fam
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
        Created At 2021-10-27 14:02:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    Stabilize sabre-compat by moving to wasm (stable)
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
        Created At 2021-10-26 21:29:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/231" class=".btn">#231</a>
            </td>
            <td>
                <b>
                    Fixups for protocol-sabre feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename protocol-sabre-exec to protocol-sabre and remove unused functions and variables from protocol::sabre.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 18:51:09 +0000 UTC
    </div>
</div>

