---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    23.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.7.2
                </span>
            </td>
            <td>
                ## 23.7.2

### Additions and Improvements
- Add new methods to `OperationTracer` to capture contexts enter/exit [#5756](https://github.com/hyperledger/besu/pull/5756)
- Add Holešky as predefined network name [#5797](https://github.com/hyperledger/besu/pull/5797)

### Breaking Changes
- Add ABI-decoded revert reason to `eth_call` and `eth_estimateGas` responses [#5705](https://github.com/hyperledger/besu/issues/5705)

### Additions and Improvements
- Add missing methods to the `Transaction` interface [#5732](https://github.com/hyperledger/besu/pull/5732)
- Add `benchmark` subcommand to `evmtool` [#5754](https://github.com/hyperledger/besu/issues/5754)
- JSON output is now compact by default. This can be overridden by the new `--json-pretty-print-enabled` CLI option. [#5766](https://github.com/hyperledger/besu/pull/5766)
- New `eth_getBlockReceipts` JSON-RPC method to retrieve all transaction receipts for a block in a single call [#5771](https://github.com/hyperledger/besu/pull/5771) 
- Add new methods to `OperationTracer` to capture contexts enter/exit [#5756](https://github.com/hyperledger/besu/pull/5756)

### Bug Fixes
- Make smart contract permissioning features work with london fork [#5727](https://github.com/hyperledger/besu/pull/5727)
- Add type to PendingTransactionDetail, fix eth_subscribe [#5729](https://github.com/hyperledger/besu/pull/5729)
- EvmTool "run" mode did not reflect contracts created within the transaction. [#5755](https://github.com/hyperledger/besu/pull/5755)
- Fixing snapsync issue with forest during the heal step [#5776](https://github.com/hyperledger/besu/pull/5776)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/23.7.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-05 22:41:50 +0000 UTC
    </span>
</div>

