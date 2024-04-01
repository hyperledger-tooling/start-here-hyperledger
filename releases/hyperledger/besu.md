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
                    24.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.4.0
                </span>
            </td>
            <td>
                ## 24.4.0

### Breaking Changes
- RocksDB database metadata format has changed to be more expressive, the migration of an existing metadata file to the new format is automatic at startup. Before performing a downgrade to a previous version it is mandatory to revert to the original format using the subcommand `besu --data-path=/path/to/besu/datadir storage revert-metadata v2-to-v1`.
- BFT networks won't start with SNAP or CHECKPOINT sync (previously Besu would start with this config but quietly fail to sync, so it's now more obvious that it won't work) [#6625](https://github.com/hyperledger/besu/pull/6625), [#6667](https://github.com/hyperledger/besu/pull/6667)
- Forest pruning has been removed, it was deprecated since 24.1.0. In case you are still using it you must now remove any of the following options: `pruning-enabled`, `pruning-blocks-retained` and `pruning-block-confirmations`, from your configuration, and you may want to consider switching to Bonsai.  

### Upcoming Breaking Changes
- Receipt compaction will be enabled by default in a future version of Besu. After this change it will not be possible to downgrade to the previous Besu version.

### Deprecations

### Additions and Improvements
- `txpool_besuPendingTransactions`change parameter `numResults` to optional parameter [#6708](https://github.com/hyperledger/besu/pull/6708)
- Extend `Blockchain` service [#6592](https://github.com/hyperledger/besu/pull/6592)
- Add bft-style `blockperiodseconds` transitions to Clique [#6596](https://github.com/hyperledger/besu/pull/6596)
- Add `createemptyblocks` transitions to Clique [#6608](https://github.com/hyperledger/besu/pull/6608)
- RocksDB database metadata refactoring [#6555](https://github.com/hyperledger/besu/pull/6555)
- Make layered txpool aware of `minGasPrice` and `minPriorityFeePerGas` dynamic options [#6611](https://github.com/hyperledger/besu/pull/6611)
- Update commons-compress to 1.26.0 [#6648](https://github.com/hyperledger/besu/pull/6648)
- Update Vert.x to 4.5.4 [#6666](https://github.com/hyperledger/besu/pull/6666)
- Refactor and extend `TransactionPoolValidatorService` [#6636](https://github.com/hyperledger/besu/pull/6636)
- Introduce `TransactionSimulationService` [#6686](https://github.com/hyperledger/besu/pull/6686)
- Transaction call object to accept both `input` and `data` field simultaneously if they are set to equal values [#6702](https://github.com/hyperledger/besu/pull/6702)
- `eth_call` for blob tx allows for empty `maxFeePerBlobGas` [#6731](https://github.com/hyperledger/besu/pull/6731)
- Extend error handling of plugin RPC methods [#6759](https://github.com/hyperledger/besu/pull/6759)
- Added engine_newPayloadV4 and engine_getPayloadV4 methods [#6783](https://github.com/hyperledger/besu/pull/6783)
- Reduce storage size of receipts [#6602](https://github.com/hyperledger/besu/pull/6602)
- Dedicated log marker for invalid txs removed from the txpool [#6826](https://github.com/hyperledger/besu/pull/6826)
- Prevent startup with BONSAI and privacy enabled [#6809](https://github.com/hyperledger/besu/pull/6809)
- Remove deprecated Forest pruning [#6810](https://github.com/hyperledger/besu/pull/6810)
- Experimental Snap Sync Server [#6640](https://github.com/hyperledger/besu/pull/6640)

### Bug fixes
- Fix txpool dump/restore race condition [#6665](https://github.com/hyperledger/besu/pull/6665)
- Make block transaction selection max time aware of PoA transitions [#6676](https://github.com/hyperledger/besu/pull/6676)
- Don't enable the BFT mining coordinator when running sub commands such as `blocks export` [#6675](https://github.com/hyperledger/besu/pull/6675)
- In JSON-RPC return optional `v` fields for type 1 and type 2 transactions [#6762](https://github.com/hyperledger/besu/pull/6762)
- Fix Shanghai/QBFT block import bug when syncing new nodes [#6765](https://github.com/hyperledger/besu/pull/6765)
- Fix to avoid broadcasting full blob txs, instead of only the tx announcement, to a subset of nodes [#6835](https://github.com/hyperledger/besu/pull/6835)
- Snap client fixes discovered during snap server testing [#6847](https://github.com/hyperledger/besu/pull/6847)

### Download Links
https://github.com/hyperledger/besu/releases/tag/24.4.0
https://github.com/hyperledger/besu/releases/download/24.4.0/besu-24.4.0.tar.gz / TBD
https://github.com/hyperledger/besu/releases/download/24.4.0/besu-24.4.0.zip / TBD

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.4.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-30 02:27:33 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.3.1
                </span>
            </td>
            <td>
                `docker pull docker.io/hyperledger/besu:24.3.1`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.3.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-30 02:27:33 +0000 UTC
    </span>
</div>

