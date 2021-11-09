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
                PR <a href="https://github.com/hyperledger/transact/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    `workload` transact CLI stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes some of the calculations in the process of turning the rate, given with the `--target-rate` CLI option, into the amount of time to wait between batch submissions. Previously starting a workload with a rate of 2/s would make the workload wait 2s between submissions making the actual rate 0.5/s
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 17:57:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    Add Isabel Tomb as a Maintainer
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
        Created At 2021-11-05 15:30:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    `family-smallbank` stabilization updates - make handler module private
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `SmallbankTransactionHandler` is already re-exported so the handler module can
be made private.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 18:37:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/251" class=".btn">#251</a>
            </td>
            <td>
                <b>
                    `family-command-workload` stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization updates for the `family-command-workload` feature
- add a module doc comment for the command::workload module
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 18:23:10 +0000 UTC
    </div>
</div>

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
                `CommandTransactionHandler` is already re-exported so the handler module can
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

