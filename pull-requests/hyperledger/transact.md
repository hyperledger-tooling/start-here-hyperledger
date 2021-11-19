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

