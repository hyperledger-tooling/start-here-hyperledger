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

