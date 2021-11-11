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
                PR <a href="https://github.com/hyperledger/transact/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    `workload-runner` stabilization updates - fix batch status check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR modifies the process in which batch statuses are checked when running a workload.

Previously the process to check the statuses of submitted batches was to call the `check_batch_status` function at the end of each loop in the `Worker` thread. However, because it takes a while for batches to be processed and return their status, the list of batch status links that needed to be checked each loop got very long after running a workload for a short period of time and slowed down the workload substantially. 

This PR changes this process to use a thread instead. This way the process can run in parallel with the worker thread and doesn't require the worker thread to wait for the statuses to be checked each iteration of the loop. The worker thread and the batch status checker thread share a `ExpectedBatchResults` hashmap so that the worker can add links to the list as batches are submitted and the batch status checker can check the links and then remove them once the status of a batch has been confirmed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 01:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    Stabilize "workload" by moving to stable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the "workload" feature by moving it to stable
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 21:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    Append -experimental to packages with experimental features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Without this commit, it's impossible to differentiate packages built
with experimental features without installing the package and running
commands to test.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 16:27:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Retire Eloá Franca Verona from maintainers
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
        Created At 2021-11-09 16:17:03 +0000 UTC
    </div>
</div>

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

