---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


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

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.7.2/besu-23.7.2.tar.gz / sha256: f74b32c1a343cbad90a88aa59276b4c5eefea4643ee542aba2bbf898f85ae242
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.7.2/besu-23.7.2.zip / sha256: a233c83591fc277e3d1530c84bb5ea896abad717d796b5e3b856c79199132b75

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.7.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-05 20:31:29 +0000 UTC
    </span>
</div>

