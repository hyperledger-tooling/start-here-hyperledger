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
                    23.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.4.0
                </span>
            </td>
            <td>
                ## 23.4.0

This quarterly update is a recommended update for stakers, but should be carefully reviewed by private network users before upgrading. This quarterly release contains a lot of new improvements but many breaking changes. We have deprecated GoQuorum-compatible privacy modes in this release, as well as IBFT1.0. If you require these, please consider migrating to new consensus algorithms or waiting for future releases. 

Highlights in this release include: 
- RocksDB 8 upgrade that improves the performance of the underlying database.
- Many logging and metrics improvements across the client.
- EVM performance improvements.
- An improved gas estimation algorithm.
- Fixes for QBFT and IBFT using zeroBaseFee
- RPC fixes 
- Many more.

Lastly, this release formalizes a deprecation notice for GoQuorum -compatible permissioning modes in Besu. These will be removed in the 23.7 series, unless otherwise stated.

### Breaking Changes
- In `evmtool` (an offline EVM executor tool principally used for reference tests), the `--prestate` and `--genesis` options no longer parse genesis files containing IBFT, QBFT, and Clique network definitions. The same genesis files will work with those json entries removed. [#5192](https://github.com/hyperledger/besu/pull/5192)
- In `--ethstats`, if the port is not specified in the URI, it will default to 443 and 80 for ssl and non-ssl connections respectively instead of 3000. [#5301](https://github.com/hyperledger/besu/pull/5301)
- Remove IBFT 1.0 feature [#5302](https://github.com/hyperledger/besu/pull/5302)
- Remove GoQuorum-compatible privacy feature [#5303](https://github.com/hyperledger/besu/pull/5303)
- Remove non-maintained launcher command line utility [#5355](https://github.com/hyperledger/besu/pull/5355)
- Remove deprecated `tx-pool-future-max-by-account` option, see instead: `tx-pool-limit-by-account-percentage` [#5361](https://github.com/hyperledger/besu/pull/5361)
- Default configuration for the deprecated ECIP-1049 network has been removed from the CLI network list [#5371](https://github.com/hyperledger/besu/pull/5371)
- GoQuorum-compatible permissioning is deprecated and will be removed in 23.7

### Additions and Improvements
- An alternate build target for the EVM using GraalVM AOT compilation was added.  [#5192](https://github.com/hyperledger/besu/pull/5192)
- To generate the binary install and use GraalVM 23.3.r17 or higher and run `./gradlew nativeCompile`.  The binary will be located in `ethereum/evmtool/build/native/nativeCompile`
- Upgrade RocksDB version from 7.7.3 to 8.0.0. Besu Team [contributed](https://github.com/facebook/rocksdb/pull/11099) to this release to make disabling checksum verification work. [#5262](https://github.com/hyperledger/besu/pull/5262)
- Log an error with stacktrace when RPC responds with internal error [#5288](https://github.com/hyperledger/besu/pull/5288)
- `--ethstats-cacert` to specify root CA of ethstats server (useful for non-production environments). [#5301](https://github.com/hyperledger/besu/pull/5301)
- Update most dependencies to latest version [#5269](https://github.com/hyperledger/besu/pull/5269)
- If jemalloc is used, print its version in the configuration overview [#4738](https://github.com/hyperledger/besu/pull/4738)
- Add metrics for accounts and storage reads (Flat database vs Merkle Patricia Trie) [#5315](https://github.com/hyperledger/besu/pull/5315)
- Offload LogBloom cache generation to computation executor, to avoid interfere with other scheduled tasks [#4530](https://github.com/hyperledger/besu/pull/4530)
- Reference tests are upgraded to use v12.1 of the ethereum tests [#5343](https://github.com/hyperledger/besu/pull/5343)
- Add new sepolia bootnodes, which should improve peering in the testnet. [#5352](https://github.com/hyperledger/besu/pull/5352)
- Renamed `--bonsai-maximum-back-layers-to-load` option to `--bonsai-historical-block-limit` for clarity. Removed `--Xbonsai-use-snapshots` option as it is no longer functional [#5337](https://github.com/hyperledger/besu/pull/5337)
- Change Forest to use TransactionDB instead of OptimisticTransactionDB [#5328](https://github.com/hyperledger/besu/pull/5328)
- Performance: Reduced usage of UInt256 in EVM operations [#5331](https://github.com/hyperledger/besu/pull/5331)
- Changed wrong error message "Invalid params" when private tx is reverted to "Execution reverted" with correct revert reason in data. [#5369](https://github.com/hyperledger/besu/pull/5369)
- Changes to the way gas is estimated to provide an exact gas estimate [#5142](https://github.com/hyperledger/besu/pull/5142)
- Add zero reads to Bonsai TrieLogs [#5317](https://github.com/hyperledger/besu/pull/5317) 
- Bonsai TrieLog serialization interface and default implementation [#5372](https://github.com/hyperledger/besu/pull/5372) 

### Bug Fixes
- Fix eth_getBlockByNumber cache error for latest block when called during syncing [#5292](https://github.com/hyperledger/besu/pull/5292)
- Fix QBFT and IBFT unable to propose blocks on London when zeroBaseFee is used [#5276](https://github.com/hyperledger/besu/pull/5276) 
- Make QBFT validator smart contract mode work with london fork [#5249](https://github.com/hyperledger/besu/issues/5249)
- Try to connect to EthStats server by default with ssl followed by non-ssl. [#5301](https://github.com/hyperledger/besu/pull/5301)
- Allow --miner-extra-data to be used in Proof-of-Stake block production [#5291](https://github.com/hyperledger/besu/pull/5291)
- Add withdrawals to payloadId calculation to avoid collisions [#5321](https://github.com/hyperledger/besu/pull/5321) 

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.4.0/besu-23.4.0.zip / sha256: 023a267ee07ed6e069cb15020c1c0262efc5ea0a3e32adc6596068cff7fd0be5
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.4.0/besu-23.4.0.tar.gz / sha256: 821695b3255c9f646f4d527e374219c96416f498231520f2eec2bebedc53f5a0


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.4.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-04-28 17:18:58 +0000 UTC
    </span>
</div>

