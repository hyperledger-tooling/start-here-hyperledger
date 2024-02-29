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
                    24.2.0-RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.2.0-RC3
                </span>
            </td>
            <td>
                ## 24.2.0-RC3

**24.2.0 is Dencun-fork-ready** for Ethereum Mainnet, which happens on March 13th! **Please make sure to upgrade your node to at least version 24.1.2 before that time, or your node will no longer follow the chain.** This is a large release with many breaking changes to Besu configurations. Please **carefully** read the following notes before you update your node. 

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
- Release docker images now provided at ghcr.io instead of dockerhub

### Deprecations
- X_SNAP and X_CHECKPOINT are marked for deprecation and will be removed in 24.4.0 in favor of SNAP and CHECKPOINT [#6405](https://github.com/hyperledger/besu/pull/6405)
- `--Xp2p-peer-lower-bound` is deprecated. [#6501](https://github.com/hyperledger/besu/pull/6501)

### Upcoming Breaking Changes
- In a future release, `--Xbonsai-limit-trie-logs-enabled` will be renamed to `--bonsai-limit-trie-logs-enabled` instead. Additionally, this limit will change to be enabled by default.
  - If you do not want the limit enabled (eg you have `--bonsai-historical-block-limit` set < 512), you need to explicitly disable it using `--bonsai-limit-trie-logs-enabled=false` or increase the limit. [#6561](https://github.com/hyperledger/besu/pull/6561)

### Additions and Improvements
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
- X_SNAP and X_CHECKPOINT are marked for deprecation and will be removed in 24.4.0
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

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.1.2...24.2.0-RC3

### Download Info

bca5bc09ca726408fe34e0b11f76d8c28526f162ecfef279c3342b4fec2b8012  besu-24.2.0-RC3.zip
ef1679cb41151ce0aa35a776fda399a8c75955b732d519bcf7e179552fb9f1c0  besu-24.2.0-RC3.tar.gz

`docker pull ghcr.io/hyperledger/besu:24.2.0-RC3`

**24.2.0-RC1 AND 24.2.0-RC2 Have been found to be bad releases. Info will be preserved, however artifacts have been removed. Please use 24.1.2 or use RC3**

ef1679cb41151ce0aa35a776fda399a8c75955b732d519bcf7e179552fb9f1c0  besu-24.2.0-RC3.tar.gz
bca5bc09ca726408fe34e0b11f76d8c28526f162ecfef279c3342b4fec2b8012  besu-24.2.0-RC3.zip

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.2.0-RC3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-02-29 01:29:16 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.2.0
                </span>
            </td>
            <td>
                

**24.2.0 is Dencun-fork-ready** for Ethereum Mainnet, which happens on March 13th! **Please make sure to upgrade your node to at least version 24.1.2 before that time, or your node will no longer follow the chain.** This is a large release with many breaking changes to Besu configurations. Please **carefully** read the following notes before you update your node. 

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
- Release docker images now provided at ghcr.io instead of dockerhub

### Deprecations
- X_SNAP and X_CHECKPOINT are marked for deprecation and will be removed in 24.4.0 in favor of SNAP and CHECKPOINT [#6405](https://github.com/hyperledger/besu/pull/6405)
- `--Xsnapsync-synchronizer-flat-db-healing-enabled` is deprecated (always enabled). [#6499](https://github.com/hyperledger/besu/pull/6499)
- `--Xp2p-peer-lower-bound` is deprecated. [#6501](https://github.com/hyperledger/besu/pull/6501)

### Upcoming Breaking Changes
- In a future release, `--Xbonsai-limit-trie-logs-enabled` will be renamed to `--bonsai-limit-trie-logs-enabled` instead. Additionally, this limit will change to be enabled by default.
  - If you do not want the limit enabled (eg you have `--bonsai-historical-block-limit` set < 512), you need to explicitly disable it using `--bonsai-limit-trie-logs-enabled=false` or increase the limit. [#6561](https://github.com/hyperledger/besu/pull/6561)

### Additions and Improvements
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
- X_SNAP and X_CHECKPOINT are marked for deprecation and will be removed in 24.4.0
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

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.1.2...24.2.0

### Download Info

2438d67593a1475257d036bcb1d8ca233384ca94f9e96481a07129abc00dc6ce  besu-24.2.0.tar.gz
e07b0047efc55dabafaa7bdf0cc83a79c866b767f385a9950c6504382d728627  besu-24.2.0.zip

`docker pull docker.io/hyperledger/besu:24.2.0`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.2.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-02-27 16:29:26 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.2.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.2.0-RC2
                </span>
            </td>
            <td>
                ## 24.2.0-RC2 Has been found to be a bad release. Artifacts have been removed, bad hashes are still included below. Please use 24.1.2 or 24.2.0-RC3

### Download Info

besu-24.2.0-RC2.tar.gz
besu-24.2.0-RC2.zip

~~docker pull ghcr.io/hyperledger/besu:24.2.0-RC2~~

**24.2.0-RC2 Has been found to be a bad release. This page will be preserved, however artifacts have been removed. Please use 24.1.2 or use RC3**

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.2.0-RC2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-02-22 14:32:54 +0000 UTC
    </span>
</div>

