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
                    22.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.10.0
                </span>
            </td>
            <td>
                ## 22.10.0

### Breaking Changes
- Flexible Privacy Groups (early access) support to Tessera's EC encryptor (contracts modified) [#4282](https://github.com/hyperledger/besu/pull/4282)
  * Before this change, the `bytes32` type was used for the enclave public keys, just supporting encryptors with public keys of that length (like the default NaCl)
  * For the EC encryptor, the encoded public key length is 91
- `--tx-pool-hashes-max-size` option removed (deprecated in 22.1.3)
- `--Xmerge-support` option remove (deprecated in 22.4.2) [#4518](https://github.com/hyperledger/besu/pull/4518)
- Breaking API changes in the `OperationTracer` interface to enable performance work.
  * The `traceExecution` method has been replaced with `tracePreExecution` and `tracePostExecution` methods, called just before and just after operation execution.
  * See `DebugOperationTracer` and `StandardJsonTracer` for migration examples.
  * RocksDB will not be able to downgrade after updating to 22.10.0 if you are looking to return to 22.7.x without a resync. Will will be changing this behavior in a future update. 

### Additions and Improvements
- Updated jackson-databind library to version 2.13.4.2 addressing [CVE-2022-42003](https://nvd.nist.gov/vuln/detail/CVE-2022-42003)
- Update snapsync feature to avoid restarting the download of the world state from scratch when restarting Besu [#4381](https://github.com/hyperledger/besu/pull/4381)
- Added worldstate snapshot isolation to improve the stability of bonsai (`--Xbonsai-use-snapshots=true`) [#4351](https://github.com/hyperledger/besu/pull/4531)
- Reduce the number of runtime exceptions (SecurityModuleException) and unnecessary executions during ECIES handshake, by trying to decrypt EIP-8 formatted messages first [#4508](https://github.com/hyperledger/besu/pull/4508).
- Improved RLP processing of zero-length string as 0x80 [#4283](https://github.com/hyperledger/besu/pull/4283) [#4388](https://github.com/hyperledger/besu/issues/4388)
- Increased level of detail in JSON-RPC parameter error log messages [#4510](https://github.com/hyperledger/besu/pull/4510)
- New unstable configuration options to set the maximum time, in milliseconds, a PoS block creation jobs is allowed to run [#4519](https://github.com/hyperledger/besu/pull/4519)
- Tune EthScheduler thread pools to avoid recreating too many threads [#4529](https://github.com/hyperledger/besu/pull/4529)
- RocksDB snapshot based worldstate and plugin-api addition of Snapshot interfaces [#4409](https://github.com/hyperledger/besu/pull/4409)
- Continuously try to build better block proposals until timeout or GetPayload is called [#4516](https://github.com/hyperledger/besu/pull/4516)
- Upgrade RocksDB database version from 6.29.5 to 7.6.0 [#4517](https://github.com/hyperledger/besu/pull/4517)
- Avoid connecting to self when using static-nodes [#4521](https://github.com/hyperledger/besu/pull/4521)
- EVM performance has increased 20%-100% depending on the particulars of the contract. [#4540](https://github.com/hyperledger/besu/pull/4540)
- Improve calculateRootHash method performance during Block processing [#4568](https://github.com/hyperledger/besu/pull/4568)
- Bring GraphQL into compliance with execution-api specs [#4112](https://github.com/hyperledger/besu/pull/4112)
- Refactor unverified forkchoice event [#4487](https://github.com/hyperledger/besu/pull/4487)
- Improve UX of initial sync logs, pushing not relevant logs to debug level [#4486](https://github.com/hyperledger/besu/pull/4486)
- Optimize pivot block selector on PoS networks [#4488](https://github.com/hyperledger/besu/pull/4488)
- Optimize Snap sync on PoS networks [#4462](https://github.com/hyperledger/besu/pull/4462)

### Bug Fixes
- Fixed default fromBlock value and improved parameter interpretation in eth_getLogs RPC handler [#4513](https://github.com/hyperledger/besu/pull/4513)
- Fix for NoSuchElementException for missing invalid reason when rejecting a local sent transaction [#4569](https://github.com/hyperledger/besu/pull/4569) 
- Corrects treating a block as bad on internal error during either validation or processing [#4512](https://github.com/hyperledger/besu/issues/4512)
- Corrects emission of blockadded events when rewinding during a re-org. Fix for [#4495](https://github.com/hyperledger/besu/issues/4495)
- Always return a transaction type for pending transactions [#4364](https://github.com/hyperledger/besu/pull/4364)
- Avoid a cyclic reference while printing EngineExchangeTransitionConfigurationParameter [#4357](https://github.com/hyperledger/besu/pull/4357)
- Corrects treating a block as bad on internal error [#4512](https://github.com/hyperledger/besu/issues/4512)
- In GraphQL update scalar parsing to be variable friendly [#4522](https://github.com/hyperledger/besu/pull/4522)
- Initiate connection to maintained peers soon after startup. [#4469](https://github.com/hyperledger/besu/pull/4469)
- Update apache-commons-text to 1.10.0 to address CVE-2022-42889 [#4542](https://github.com/hyperledger/besu/pull/4542)

### Download Links

https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.10.0/besu-22.10.0.tar.gz  / sha256: 18590796831a6c6c2ca17ba8e6877dd2bd63c25e034f1bbc987aaa0a9c3a178e
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.10.0/besu-22.10.0.zip / sha256: 8ad4927469e8e128a3a2c7a708f108393eebc82c522f66cdcac4b7d206e07f90 
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.10.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-02 18:01:59 +0000 UTC
    </span>
</div>

