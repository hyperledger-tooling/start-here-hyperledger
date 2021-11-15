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
                PR <a href="https://github.com/hyperledger/transact/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    `family-command-workload` stabilization updates - add CommandTransactionBuilder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace `make_command_transaction` with `CommandTransactionBuilder`.

```
let command_transaction_pair: TransactionPair = CommandTransactionBuilder::new()
  .with_commands(vec![commands])
  .into_transaction_builder()?
  .build_pair()?;
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 03:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    `workload-runner` stabilization - request logger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization updates for the `workload-runner` feature in libtransact

The main focus of this PR is to move the printing functionality of `HttpRequestCounter` to the CLI. This PR replaces the `log` function in `HttpRequestCounter` with a `RequestLogger` in the CLI which takes a list of `HttpRequestCounter`s and starts a thread which loops through the counters, printing the information stored in them. The request logger uses the value given with the `--update` option to sleep for the correct amount of time between logs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 00:07:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    `family-command` stabilization updates - Add documentation for handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add documentation for `CommandTransactionHandler`

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 00:06:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    `family-smallbank` stabilization updates - Add API doc for handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add API doc for the `SmallbankTransactionHandler`

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 23:40:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    `workload-batch-gen` stabilization updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilization updates for the "workload-batch-gen" feature

- Remove `SignedBatchIterator` because it isn't used
- Make `BatchListFeeder` pub(super) 
- Make `BatchListResult` type pub(super) 
- Remove unused variants from `BatchReadingError`
- Replace `generate_signed_batches` with a `write_to` function for `SignedBatchProducer` and update cli playlist to use it
- Make BatchResult type private
- Modify the `batch_transactions` function to use `BatchBuilder` to eliminate the need to use protobuf directly
- Add feature guards to `BatchingError` and replace the `BatchingError` variants with common errors `InternalError` and
`InvalidStateError`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 18:48:22 +0000 UTC
    </div>
</div>

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

