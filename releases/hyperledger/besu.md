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
                    24.5.2-RC0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.5.2-RC0
                </span>
            </td>
            <td>
                ### Additions and Improvements
- Remove deprecated Goerli testnet [#7049](https://github.com/hyperledger/besu/pull/7049)
- Default bonsai to use full-flat db and code-storage-by-code-hash [#6984](https://github.com/hyperledger/besu/pull/6894)
- New RPC methods miner_setExtraData and miner_getExtraData [#7078](https://github.com/hyperledger/besu/pull/7078)
- Disconnect peers that have multiple discovery ports since they give us bad neighbours [#7089](https://github.com/hyperledger/besu/pull/7089)

### Bug fixes
- Fix parsing `gasLimit` parameter when its value is > `Long.MAX_VALUE` [#7116](https://github.com/hyperledger/besu/pull/7116)
- Skip validation of withdrawals when importing BFT blocks since withdrawals don't apply to BFT chains [#7115](https://github.com/hyperledger/besu/pull/7115)

## New Contributors
* @knowmost made their first contribution in https://github.com/hyperledger/besu/pull/7005
* @seanyoung made their first contribution in https://github.com/hyperledger/besu/pull/7054

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.5.1...24.5.2-RC0
c3a702915556fdea16968c0924783d939f50863b561d27e565fe9ae9e0edd815  besu-24.5.2-RC0.tar.gz
2100ff8764d3cfa85aa259467d537bbc9fa08259e3036b8deb7e68eaf8e54dd8  besu-24.5.2-RC0.zip

`docker pull docker.io/hyperledger/besu:24.5.2-RC0`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.5.2-RC0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-17 01:54:19 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.5.0
                </span>
            </td>
            <td>
                Due to a GHA quirk, this release is deprecated in favour of https://github.com/hyperledger/besu/releases/tag/24.5.1


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.5.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-13 23:23:15 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.5.1
                </span>
            </td>
            <td>
                ## What's Changed
There's a lot in this release, notably 
* early access Snap Sync Server
* reduction in storage size of receipt
* optional `v` fields for type 1 and type 2 transactions

Note there are 2 known issues which we are still working on (details below).

### Breaking Changes
- RocksDB database metadata format has changed to be more expressive, the migration of an existing metadata file to the new format is automatic at startup. Before performing a downgrade to a previous version it is mandatory to revert to the original format using the subcommand `besu --data-path=/path/to/besu/datadir storage revert-metadata v2-to-v1`.
- BFT networks won't start with SNAP or CHECKPOINT sync (previously Besu would start with this config but quietly fail to sync, so it's now more obvious that it won't work) [#6625](https://github.com/hyperledger/besu/pull/6625), [#6667](https://github.com/hyperledger/besu/pull/6667)
- Forest pruning has been removed, it was deprecated since 24.1.0. In case you are still using it you must now remove any of the following options: `pruning-enabled`, `pruning-blocks-retained` and `pruning-block-confirmations`, from your configuration, and you may want to consider switching to Bonsai.

### Upcoming Breaking Changes
- Version 24.5.x will be the last series to support Java 17. Next release after versions 24.5.x will require Java 21 to build and run.
- Receipt compaction will be enabled by default in a future version of Besu. After this change it will not be possible to downgrade to the previous Besu version.
- PKI-backed QBFT will be removed in a future version of Besu. Other forms of QBFT will remain unchanged.

### Known Issues
- [Frequency: occasional < 10%] Chain download halt. Only affects new syncs (new nodes syncing from scratch). Symptom: Block import halts, despite having a full set of peers and world state downloading finishing. Generally restarting besu will resolve the issue. We are tracking this in [#6884](https://github.com/hyperledger/besu/pull/6884)
- [Frequency: occasional < 10%] Low peer numbers. More likely to occur on testnets (holesky and sepolia) but also can occur on mainnet. Symptom: peer count stays at 0 for an hour or more. Generally restarting besu will resolve the issue. We are tracking this in [#6805](https://github.com/hyperledger/besu/pull/6805)


### Additions and Improvements
- Update "host allow list" logic to transition from deprecated `host()` method to suggested `authority()` method.[#6878](https://github.com/hyperledger/besu/issues/6878)
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
- Upgrade Reference Tests to 13.2 [#6854](https://github.com/hyperledger/besu/pull/6854)
- Update Web3j dependencies [#6811](https://github.com/hyperledger/besu/pull/6811)
- Add `tx-pool-blob-price-bump` option to configure the price bump percentage required to replace blob transactions (by default 100%) [#6874](https://github.com/hyperledger/besu/pull/6874)
- Log detailed timing of block creation steps [#6880](https://github.com/hyperledger/besu/pull/6880)
- Expose transaction count by type metrics for the layered txpool [#6903](https://github.com/hyperledger/besu/pull/6903)
- Expose bad block events via the BesuEvents plugin API  [#6848](https://github.com/hyperledger/besu/pull/6848)
- Add RPC errors metric [#6919](https://github.com/hyperledger/besu/pull/6919/)
- Add `rlp decode` subcommand to decode IBFT/QBFT extraData to validator list [#6895](https://github.com/hyperledger/besu/pull/6895)
- Allow users to specify which plugins are registered [#6700](https://github.com/hyperledger/besu/pull/6700)
- Layered txpool tuning for blob transactions [#6940](https://github.com/hyperledger/besu/pull/6940)

### Bug fixes
- Fix txpool dump/restore race condition [#6665](https://github.com/hyperledger/besu/pull/6665)
- Make block transaction selection max time aware of PoA transitions [#6676](https://github.com/hyperledger/besu/pull/6676)
- Don't enable the BFT mining coordinator when running sub commands such as `blocks export` [#6675](https://github.com/hyperledger/besu/pull/6675)
- In JSON-RPC return optional `v` fields for type 1 and type 2 transactions [#6762](https://github.com/hyperledger/besu/pull/6762)
- Fix Shanghai/QBFT block import bug when syncing new nodes [#6765](https://github.com/hyperledger/besu/pull/6765)
- Fix to avoid broadcasting full blob txs, instead of only the tx announcement, to a subset of nodes [#6835](https://github.com/hyperledger/besu/pull/6835)
- Snap client fixes discovered during snap server testing [#6847](https://github.com/hyperledger/besu/pull/6847)
- Correctly initialize the txpool as disabled on creation [#6890](https://github.com/hyperledger/besu/pull/6890)
- Fix worldstate download halt when using snap sync during initial sync [#6981](https://github.com/hyperledger/besu/pull/6981)
- Fix chain halt due to peers only partially responding with headers. Also worldstate halts caused by a halt in the chain sync [#7027](https://github.com/hyperledger/besu/pull/7027)

### Download Info
77e39b21dbd4186136193fc6e832ddc1225eb5078a5ac980fb754b33ad35d554  besu-24.5.1.tar.gz
13d75b6b22e1303f39fd3eaddf736b24ca150b2bafa7b98fce7c7782e54b213f  besu-24.5.1.zip

## New Contributors
* @RoboCopsGoneSock made their first contribution in https://github.com/hyperledger/besu/pull/6677
* @friedemannf made their first contribution in https://github.com/hyperledger/besu/pull/6702
* @MASDXI made their first contribution in https://github.com/hyperledger/besu/pull/6708
* @wellweek made their first contribution in https://github.com/hyperledger/besu/pull/6730
* @suraneti made their first contribution in https://github.com/hyperledger/besu/pull/6562
* @standstaff made their first contribution in https://github.com/hyperledger/besu/pull/6741
* @Savid made their first contribution in https://github.com/hyperledger/besu/pull/6744
* @lyfsn made their first contribution in https://github.com/hyperledger/besu/pull/6758
* @StevenMia made their first contribution in https://github.com/hyperledger/besu/pull/6951
* @goodactive made their first contribution in https://github.com/hyperledger/besu/pull/6971

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.3.3...24.5.0-RC2



            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.5.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-10 02:38:37 +0000 UTC
    </span>
</div>

