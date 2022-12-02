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
                    22.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.10.1
                </span>
            </td>
            <td>
                ## 22.10.1

### Breaking Changes
- Fields `publicKey` and `raw` removed from RPC API `Transaction` result object [#4575](https://github.com/hyperledger/besu/pull/4575)

### Additions and Improvements
- Explain and improve price validation for London and local transactions during block proposal selection [#4602](https://github.com/hyperledger/besu/pull/4602)
- Support for ephemeral testnet Shandong, for EOF testing. [#4599](https://github.com/hyperledger/besu/pull/4599)
- Improve performance of block processing by parallelizing some parts during the "commit" step [#4635](https://github.com/hyperledger/besu/pull/4635)
- Upgrade RocksDB version from 7.6.0 to 7.7.3
- Added new RPC endpoints `debug_setHead` & `debug_replayBlock`  [4580](https://github.com/hyperledger/besu/pull/4580)
- Upgrade OpenTelemetry to version 1.19.0 [#3675](https://github.com/hyperledger/besu/pull/3675)
- Implement Eth/67 sub-protocol [#4596](https://github.com/hyperledger/besu/issues/4596)
- Backward sync log UX improvements [#4655](https://github.com/hyperledger/besu/pull/4655)
- Enable RocksDB Bloom filters to improve read performance [#4682](https://github.com/hyperledger/besu/pull/4682)
- Backward sync: use retry switching peer when fetching data from peers [#4656](https://github.com/hyperledger/besu/pull/4656)
- Shanghai implementation of EIP-3651 Warm coinbase [#4620](https://github.com/hyperledger/besu/pull/4620) 
- Shanghai implementation of EIP-3855 Push0 [#4660](https://github.com/hyperledger/besu/pull/4660)
- Shanghai implementation of EIP-3540 and EIP-3670 Ethereum Object Format and Code Validation [#4644](https://github.com/hyperledger/besu/pull/4644)
- Remove some log statements that are keeping some objects live in heap for a long time, to reduce the amount of memory required during initial sync [#4705](https://github.com/hyperledger/besu/pull/4705)
- Add field `type` to Transaction receipt object (eth_getTransactionReceipt) [#4505](https://github.com/hyperledger/besu/issues/4505)
- Print an overview of configuration and system information at startup [#4451](https://github.com/hyperledger/besu/pull/4451)
- Do not send new payloads to backward sync if initial sync is in progress [#4720](https://github.com/hyperledger/besu/issues/4720)
- Improve the way transaction fee cap validation is done on London fee market to not depend on transient network conditions [#4598](https://github.com/hyperledger/besu/pull/4598) 
- Preload and cache account and storage data from RocksDB to improve performance  [#4737](https://github.com/hyperledger/besu/issues/4737)

### Bug Fixes
- Restore updating chain head and finalized block during backward sync [#4718](https://github.com/hyperledger/besu/pull/4718)

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.10.1/besu-22.10.1.tar.gz  / sha256: b6757b9fc69b782cdabb95b1e784d31b1effcc2e25c6b198b2f9d6b3786c7a8a
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.10.1/besu-22.10.1.zip / sha256: 0dbee534620c7cc0fac0596e6df0c7f8a74be9df9cecd9d4f1407016f30fb9a1

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.10.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-12-01 22:27:28 +0000 UTC
    </span>
</div>

