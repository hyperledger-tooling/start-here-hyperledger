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
                    21.7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.7.3
                </span>
            </td>
            <td>
                
### Additions and Improvements
- Migration to Apache Tuweni 2.0 [\#2376](https://github.com/hyperledger/besu/pull/2376)
- \[EXPERIMENTAL\] Added support for DevP2P-over-TLS [#2536](https://github.com/hyperledger/besu/pull/2536)
- `eth_getWork`, `eth_submitWork` support over the Stratum port [#2581](https://github.com/hyperledger/besu/pull/2581)
- Stratum metrics [#2583](https://github.com/hyperledger/besu/pull/2583)
- Support for mining ommers [#2576](https://github.com/hyperledger/besu/pull/2576)
- Updated onchain permissioning to validate permissions on transaction submission [\#2595](https://github.com/hyperledger/besu/pull/2595)
- Removed deprecated CLI option `--privacy-precompiled-address` [#2605](https://github.com/hyperledger/besu/pull/2605)
- Removed code supporting EIP-1702. [#2657](https://github.com/hyperledger/besu/pull/2657)
- A native library was added for the alternative signature algorithm secp256r1, which will be used by default [#2630](https://github.com/hyperledger/besu/pull/2630)
- The command line option --Xsecp-native-enabled was added as an alias for --Xsecp256k1-native-enabled [#2630](https://github.com/hyperledger/besu/pull/2630)
- Added Labelled gauges for metrics [#2646](https://github.com/hyperledger/besu/pull/2646)
- support for `eth/66` networking protocol [#2365](https://github.com/hyperledger/besu/pull/2365)
- update RPC methods for post london 1559 transaction [#2535](https://github.com/hyperledger/besu/pull/2535)
- \[EXPERIMENTAL\] Added support for using DNS host name in place of IP address in onchain node permissioning rules [#2667](https://github.com/hyperledger/besu/pull/2667)
- Implement EIP-3607 Reject transactions from senders with deployed code. [#2676](https://github.com/hyperledger/besu/pull/2676)
- Ignore all unknown fields when supplied to eth_estimateGas or eth_call. [\#2690](https://github.com/hyperledger/besu/pull/2690)

### Bug Fixes
- Consider effective price and effective priority fee in transaction replacement rules [\#2529](https://github.com/hyperledger/besu/issues/2529)
- GetTransactionCount should return the latest transaction count if it is greater than the transaction pool [\#2633](https://github.com/hyperledger/besu/pull/2633) 

### Download Link
[https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/21.7.3/besu-21.7.3.zip](https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/21.7.3/besu-21.7.3.zip)\
SHA256: 676c8bbcf4a2e7d08198b0a106a2164e8d55d6f3e1d19783cfd70048be302fb3

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/21.7.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-09-02 22:39:49 +0000 UTC
    </span>
</div>

