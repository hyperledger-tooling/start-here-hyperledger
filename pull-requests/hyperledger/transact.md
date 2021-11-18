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
                - Update the content of the command get-state man page.
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Fix feature guard on static adapter tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change the feature guard on the tests in the `static_adapter` module from "family-command" to "family-command-workload", the tests use `CommandTransactionBuilder` which is behind the "family-command-workload" feature.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 17:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    Stabilize `family-command`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the "family-command" feature by moving it from experimental
to stable.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 16:30:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Stabilize `family-smallbank`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the "family-smallbank" feature by moving it from experimental
to stable.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 16:22:55 +0000 UTC
    </div>
</div>

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
                family-command-workload stabilization updates:

- Replace `make_command_transaction` with `CommandTransactionBuilder`. CommandTransactionBuilder can be used in the following way to create command transactions:

```
let command_transaction_pair: TransactionPair = CommandTransactionBuilder::new()
  .with_commands(vec![commands])
  .into_transaction_builder()?
  .build_pair()?;
```
- Remove pub from `playlist::bytes_to_hex_str`
- Refactor the `CommandGeneratingIter` to remove panics
- Rename the `playlist` module in `families::command::workload` to `command_iter` as it does not contain any playlist related code
- Refactor code to only use protocol to avoid using protobuf directly
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

