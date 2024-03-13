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
                    develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    develop
                </span>
            </td>
            <td>
                This is an automated, bleeding edge build from the tip of main. No promises. YOLO.

23d3a2327fd3c4f0afc66d3a6159a846f9590d022b356f17f2a041689dcc4b21  besu-24.3-develop-39a356f824.tar.gz
9eb212e60a7938bcefa8fd15fb651f9d70cb8f44f8c4cfa5b98e0af00af3030e  besu-24.3-develop-39a356f824.zip

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/develop" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-12 22:24:22 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.3.0
                </span>
            </td>
            <td>
                ## 24.3.0

**24.3.0 is Dencun-fork-ready** for Ethereum Mainnet, which happens on March 13th! **Please make sure to upgrade your node to at least version 24.1.2 before that time, or your node will no longer follow the chain.** This is a large release with many breaking changes to Besu configurations. Please **carefully** read the following notes before you update your node. 

Besu now has new, sensible defaults for public networks. BONSAI and SNAP are now default, so check your configuration if you are NOT using these as you upgrade. The database also more gracefully exits when starting up with the other storage format. 

Bonsai is also getting an upgrade to reduce overall storage usage! With a new option to limit accumulation of trie logs, you should save 3GB on state growth per week, with an option to remove old trie logs from your database. See this PR for more details [#5390](https://github.com/hyperledger/besu/issues/5390). There are a few other improvements to reduce Besu's size on disk when using Bonsai. 

With this version, QBFT now supports Shanghai OpCodes and contracts! Besu now also includes an option to restrict downgrades. This can be enabled in your config. 

Lastly, this version includes several performance improvements to the EVM and execution performance, as well as memory usage improvements in the high-spec flag. There are new APIs for Dencun and several bug fixes. See the notes below for more details. 

### Breaking Changes
- SNAP - Snap sync is now the default for named networks [#6530](https://github.com/hyperledger/besu/pull/6530)
  - if you want to use the previous default behavior, you'll need to specify `--sync-mode=FAST`
- BONSAI - Default data storage format is now Bonsai [#6536](https://github.com/hyperledger/besu/pull/6536)
  - if you had previously used the default (FOREST), at startup you will get an error indicating the mismatch
    `Mismatch: DB at '/your-path' is FOREST (Version 1) but config expects BONSAI (Version 2). Please check your config.`
  - to fix this mismatch, specify the format explicitly using `--data-storage-format=FOREST`
- Following the OpenMetrics convention, the updated Prometheus client adds the `_total` suffix to every metrics of type counter, with the effect that some existing metrics have been renamed to have this suffix. If you are using the official Besu Grafana dashboard [(available here)](https://grafana.com/grafana/dashboards/16455-besu-full/), just update it to the latest revision, that accepts the old and the new name of the affected metrics. If you have a custom dashboard or use the metrics in other ways, then you need to manually update it to support the new naming.
- The `trace-filter` method in JSON-RPC API now has a default block range limit of 1000, adjustable with `--rpc-max-trace-filter-range` (thanks @alyokaz) [#6446](https://github.com/hyperledger/besu/pull/6446)
- Requesting the Ethereum Node Record (ENR) to acquire the fork id from bonded peers is now enabled by default, so the following change has been made [#5628](https://github.com/hyperledger/besu/pull/5628):
- `--Xfilter-on-enr-fork-id` has been removed. To disable the feature use `--filter-on-enr-fork-id=false`.
- `--engine-jwt-enabled` has been removed. Use `--engine-jwt-disabled` instead. [#6491](https://github.com/hyperledger/besu/pull/6491)

### Deprecations
- X_SNAP and X_CHECKPOINT are marked for deprecation and will be removed in 24.6.0 in favor of SNAP and CHECKPOINT [#6405](https://github.com/hyperledger/besu/pull/6405)
- `--Xp2p-peer-lower-bound` is deprecated. [#6501](https://github.com/hyperledger/besu/pull/6501)

### Upcoming Breaking Changes
- In a future release, `--Xbonsai-limit-trie-logs-enabled` will be renamed to `--bonsai-limit-trie-logs-enabled` instead. Additionally, this limit will change to be enabled by default.
  - If you do not want the limit enabled (eg you have `--bonsai-historical-block-limit` set < 512), you need to explicitly disable it using `--bonsai-limit-trie-logs-enabled=false` or increase the limit. [#6561](https://github.com/hyperledger/besu/pull/6561)

### Additions and Improvements
- `eth_call` and `eth_feeHistory` add blob fields https://github.com/hyperledger/besu/pull/6681
- Improves block processing performance by precalculating transactions' sender [#6375](https://github.com/hyperledger/besu/pull/6375) and optimizing Keccak hash calculations for account storage slots during the commit phase[#6452](https://github.com/hyperledger/besu/pull/6452).
- Upgrade Prometheus and Opentelemetry dependencies [#6422](https://github.com/hyperledger/besu/pull/6422)
- Add `OperationTracer.tracePrepareTransaction`, where the sender account has not yet been altered[#6453](https://github.com/hyperledger/besu/pull/6453)
- Improve the high spec flag by limiting it to a few column families [#6354](https://github.com/hyperledger/besu/pull/6354)
- Log blob count when importing a block via Engine API [#6466](https://github.com/hyperledger/besu/pull/6466)
- Introduce `--Xbonsai-limit-trie-logs-enabled` experimental feature which by default will only retain the latest 512 trie logs, saving about 3GB per week in database growth [#5390](https://github.com/hyperledger/besu/issues/5390) 
  - See https://wiki.hyperledger.org/display/BESU/Limit+Trie+Logs+for+Bonsai for more info
- Introduce `besu storage x-trie-log prune` experimental offline subcommand which will prune all redundant trie logs except the latest 512 [#6303](https://github.com/hyperledger/besu/pull/6303)  
  - See https://wiki.hyperledger.org/display/BESU/Limit+Trie+Logs+for+Bonsai for more info
- Improve flat trace generation performance [#6472](https://github.com/hyperledger/besu/pull/6472)
- SNAP and CHECKPOINT sync - early access flag removed so now simply SNAP and CHECKPOINT [#6405](https://github.com/hyperledger/besu/pull/6405)
- X_SNAP and X_CHECKPOINT are marked for deprecation and will be removed in 24.6.0
- Github Actions based build.
- Introduce caching mechanism to optimize Keccak hash calculations for account storage slots during block processing [#6452](https://github.com/hyperledger/besu/pull/6452)
- Added configuration options for `pragueTime` to genesis file for Prague fork development [#6473](https://github.com/hyperledger/besu/pull/6473)
- Moving trielog storage to RocksDB's blobdb to improve write amplications [#6289](https://github.com/hyperledger/besu/pull/6289)
- Support for `shanghaiTime` fork and Shanghai EVM smart contracts in QBFT/IBFT chains [#6353](https://github.com/hyperledger/besu/pull/6353)
- Change ExecutionHaltReason for contract creation collision case to return ILLEGAL_STATE_CHANGE [#6518](https://github.com/hyperledger/besu/pull/6518) 
- Experimental feature `--Xbonsai-code-using-code-hash-enabled` for storing Bonsai code storage by code hash [#6505](https://github.com/hyperledger/besu/pull/6505)
- More accurate column size `storage rocksdb usage` subcommand [#6540](https://github.com/hyperledger/besu/pull/6540)
- Adds `storage rocksdb x-stats` subcommand [#6540](https://github.com/hyperledger/besu/pull/6540)
- New `eth_blobBaseFee`JSON-RPC method [#6581](https://github.com/hyperledger/besu/pull/6581)
- Upgrade reference tests to version 13.1 [#6574](https://github.com/hyperledger/besu/pull/6574)
- Extend `BesuConfiguration` service [#6584](https://github.com/hyperledger/besu/pull/6584)
- Add `ethereum_min_gas_price` and `ethereum_min_priority_fee` metrics to track runtime values of `min-gas-price` and `min-priority-fee` [#6587](https://github.com/hyperledger/besu/pull/6587)
- Option to perform version incompatibility checks when starting Besu. In this first release of the feature, if `--version-compatibility-protection` is set to true it checks that the version of Besu being started is the same or higher than the previous version. [6307](https://github.com/hyperledger/besu/pull/6307)
- Moved account frame warming from GasCalculator into the Call operations [#6557](https://github.com/hyperledger/besu/pull/6557)

### Bug fixes
- Fix the way an advertised host configured with `--p2p-host` is treated when communicating with the originator of a PING packet [#6225](https://github.com/hyperledger/besu/pull/6225)
- Fix `poa-block-txs-selection-max-time` option that was inadvertently reset to its default after being configured [#6444](https://github.com/hyperledger/besu/pull/6444)
- Fix for tx incorrectly discarded when there is a timeout during block creation [#6563](https://github.com/hyperledger/besu/pull/6563)
- Fix traces so that call gas costing in traces matches other clients traces [#6525](https://github.com/hyperledger/besu/pull/6525)

## New Contributors
* @alyokaz made their first contribution in https://github.com/hyperledger/besu/pull/6446
* @Brindrajsinh-Chauhan made their first contribution in https://github.com/hyperledger/besu/pull/6587

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.1.2...24.3.0

### Download Info


8037ce51bb5bb396d29717a812ea7ff577b0d6aa341d67d1e5b77cbc55b15f84  besu-24.3.0.tar.gz
41ea2ca734a3b377f43ee178166b5b809827084789378dbbe4e5b52bbd8e0674  besu-24.3.0.zip

`docker pull docker.io/hyperledger/besu:24.3.0`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.3.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-05 06:42:04 +0000 UTC
    </span>
</div>

