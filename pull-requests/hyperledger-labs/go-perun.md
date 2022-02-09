---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/322" class=".btn">#322</a>
            </td>
            <td>
                <b>
                    Use LatestSigner and don't set GasPrice in ContractBackend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - eth/channel: Use types.LatestSigner for all sim backend tests
  - Before, `types.EIP155Signer`s were created in many different places.
It is recommended by the geth folks to use `types.LatestSigner` instead.
This was streamlined an there's now a common `channel/test.SimSigner` that
can always be used together with the simulated backend.
  - `FundAddress` and `Test_ConfirmTransaction` were adapted to use the
new `types.DynamicFeeTx`.
  - The unused `test.GasLimit` variable was deleted.
  - The `test.GasPrice` variable was renamed to `InitialGasBaseFee` and its
description updated.
- eth/channel: Don't set `GasPrice` in `ContractBackend.NewTransactor`
  - Setting `TransactOpts.GasPrice` forces the transactions to be sent as a
legacy transaction, instead of a type 2 EIP1559, which results in much
higher gas costs.
  - Also remove the `SuggestedGasPrice` method from the `SimulatedBackend`, as
it is not used anymore, because EIP1559 TXs are now sent everywhere.

Opened as a draft to let @ndzik try it out first if we truly now send EIP1559 txs.
Original issue in Erdstall is at https://github.com/perun-network/erdstall-ext/issues/121
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 17:03:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/319" class=".btn">#319</a>
            </td>
            <td>
                <b>
                    Fix CI fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Stabilise reorg resistant subscription tests, although it does not cause the inherent problem that caused the tests to fail. Fixing that would be way more involved.
* Fix bug in Adjudicator test: challenge duration (is used as timeout for the funding transactions) was selected in *[0,3600)*, fixed to *[200,3600)* now, to guarantee enough time for funding.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 11:01:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Implement protobuf adapter for wire serialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #311

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 08:55:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Refactor message serialization tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor the tests to use generic test functions.

- In preparation for extending these tests to newer wire serialization
  adapters.

- Also, use random string for reason field in shutdowm message test.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 07:00:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    Add missing tests for sync msg serialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - These tests were missing.

Signed-off-by: Manoranjith <ponraj.manoranjitha@in.bosch.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 05:57:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/315" class=".btn">#315</a>
            </td>
            <td>
                <b>
                    channel: Init balances to zero
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a bug where balances were not initialized to zero.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 11:50:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Readme update backends
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Improves the README:
- Adds information about more available blockchain backends.
- Adds information about available documentation and code examples.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 11:44:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    client: Export proposer and proposee index
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #79 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 10:00:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Implement protobuf adapter for wire serialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - [x] Add protocol buffer definitions in ~wire/protobuf/wire.proto~ file.
- [x] Add a config file for ~/.protolint~ tool for linting *.proto files.
- [x] Add a job in github ci config for running protolint tool.
- [ ] Add generated bindings and helper functions for
  serializing/de-serializing messags to/from using protobuf wire format.
- [ ] Disable default use of ~perunio~ encoding and make provisions for the
  user to choose the adapter.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 09:46:36 +0000 UTC
    </div>
</div>

