---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Update go-perun to v0.10.3
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
        Created At 2022-08-03 06:34:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    wallet: Transactor work with newer Wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The currently used hdwallet only supports legacy (pre EIP-155) transactions. Other wallet implementations like Go-Ethereum's [Keystore Wallet](https://github.com/ethereum/go-ethereum/blob/d804a59ee1a0152e98bb8dbd5cfea522409a2a5e/accounts/keystore/keystore.go#L276-L289) expect the chainID to be nil for those legacy transactions. Thus those wallets are currently unable to sign them. When using a SimulatedBackend trying to sign a legacy transaction with a London-fork-capable wallet returns the error `invalid chain id for signer`.

The currently used hdwallet is not affected by this change, it completely ignores the third argument.

**Edit**:
I just found out that transactions created using the go bindings (BoundContract) do not set the chainID, leaving it at the default value of 0, even if newer transactions are used. (see the [createDynamicTx](https://github.com/ethereum/go-ethereum/blob/d804a59ee1a0152e98bb8dbd5cfea522409a2a5e/accounts/abi/bind/base.go#L277-L285) function). Go-Ethereum seems to happily sign them and accept them on-chain, however the signer still needs a chainID to sign them.

This means that transactions will not be signed in the following case (even with the changes in this PR):
- Wallet supports newer transaction types like DynamicFeeTransactions AND // Not the case with the currently used hdwallet
- `txn.chainID == 0` AND
- transaction type != LegacyTransaction // This condition didn't exist before this PR, since no transaction with `chainID==0` could be signed

`txn.chainID == 0` also happens if the transaction is created using bindings and `transactionOpts.GasPrice != nil` (as is the case with this Transactor.

The easiest fix for this is probably to add the chainID field to the transactor instead of reading it from the transactions, but that may have consequences for other places using the Transactor.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 16:57:32 +0000 UTC
    </div>
</div>

