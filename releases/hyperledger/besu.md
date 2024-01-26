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
                    Release 24.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.1.1
                </span>
            </td>
            <td>
                ## 24.1.1

### Breaking Changes
- New `EXECUTION_HALTED` error returned if there is an error executing or simulating a transaction, with the reason for execution being halted. Replaces the generic `INTERNAL_ERROR` return code in certain cases which some applications may be checking for [#6343](https://github.com/hyperledger/besu/pull/6343)
- The Besu Docker images with `openjdk-latest` tags since 23.10.3 were incorrectly using UID 1001 instead of 1000 for the container's `besu` user. The user now uses 1000 again. Containers created from or migrated to images using UID 1001 will need to chown their persistent database files to UID 1000 [#6360](https://github.com/hyperledger/besu/pull/6360)
- The deprecated `--privacy-onchain-groups-enabled` option has now been removed. Use the `--privacy-flexible-groups-enabled` option instead. [#6411](https://github.com/hyperledger/besu/pull/6411)
- The time that can be spent selecting transactions during block creation is not capped at 5 seconds for PoS and PoW networks, and for PoA networks, at 75% of the block period specified in the genesis, this to prevent possible DoS in case a single transaction is taking too long to execute, and to have a stable block production rate, but it could be a breaking change if an existing network used to have transactions that takes more time to executed that the newly introduced limit, if it is mandatory for these network to keep processing these long processing transaction, then the default value of `block-txs-selection-max-time` or `poa-block-txs-selection-max-time` needs to be tuned accordingly. [#6423](https://github.com/hyperledger/besu/pull/6423)

### Deprecations

### Additions and Improvements
- Optimize RocksDB WAL files, allows for faster restart and a more linear disk space utilization [#6328](https://github.com/hyperledger/besu/pull/6328)
- Disable transaction handling when the node is not in sync, to avoid unnecessary transaction validation work [#6302](https://github.com/hyperledger/besu/pull/6302)
- Introduce TransactionEvaluationContext to pass data between transaction selectors and plugin, during block creation [#6381](https://github.com/hyperledger/besu/pull/6381)
- Upgrade dependencies [#6377](https://github.com/hyperledger/besu/pull/6377)
- Upgrade `com.fasterxml.jackson` dependencies [#6378](https://github.com/hyperledger/besu/pull/6378)
- Upgrade Guava dependency [#6396](https://github.com/hyperledger/besu/pull/6396)
- Upgrade Mockito [#6397](https://github.com/hyperledger/besu/pull/6397)
- Upgrade `tech.pegasys.discovery:discovery` [#6414](https://github.com/hyperledger/besu/pull/6414)
- Options to tune the max allowed time that can be spent selecting transactions during block creation are now stable [#6423](https://github.com/hyperledger/besu/pull/6423)

### Bug fixes
- INTERNAL_ERROR from `eth_estimateGas` JSON/RPC calls [#6344](https://github.com/hyperledger/besu/issues/6344)
- Fix Besu Docker images with `openjdk-latest` tags since 23.10.3 using UID 1001 instead of 1000 for the `besu` user [#6360](https://github.com/hyperledger/besu/pull/6360)
- Fluent EVM API definition for Tangerine Whistle had incorrect code size validation configured [#6382](https://github.com/hyperledger/besu/pull/6382)
- Correct mining beneficiary for Clique networks in TraceServiceImpl [#6390](https://github.com/hyperledger/besu/pull/6390)
- Fix to gas limit delta calculations used in block production. Besu should now increment or decrement the block gas limit towards its target correctly (thanks @arbora) #6425
- Ensure Backward Sync waits for initial sync before starting a session [#6455](https://github.com/hyperledger/besu/issues/6455)
- Silence the noisy DNS query errors [#6458](https://github.com/hyperledger/besu/issues/6458)

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.zip / sha256 e23c5b790180756964a70dcdd575ee2ed2c2efa79af00bce956d23bd2f7dc67c
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.tar.gz / sha256 4b0ddd5a25be2df5d2324bff935785eb63e4e3a5f421614ea690bacb5b9cb344

### Errata
Note, due to a CI race with the release job, the initial published version of 24.1.1 were overwritten by artifacts generated from the same sources, but differ in their embedded timestamps.  The initial SHAs are noted here but are deprecated:
~~https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.zip / sha256 b6b64f939e0bb4937ce90fc647e0a7073ce3e359c10352b502059955070a60c6~~
~~https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.1/besu-24.1.1.tar.gz / sha256 cfcae04c30769bf338b0740ac65870f9346d3469931bb46cdba3b2f65d311e7a~~

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.1.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-01-26 01:04:20 +0000 UTC
    </span>
</div>

