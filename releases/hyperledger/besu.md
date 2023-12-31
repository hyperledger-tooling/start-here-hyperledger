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
                    23.10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.10.3
                </span>
            </td>
            <td>
                ## 23.10.3

### Additions and Improvements
- Implement debug_traceCall [#5885](https://github.com/hyperledger/besu/pull/5885)
- Transactions that takes too long to evaluate, during block creation, are dropped from the txpool [#6163](https://github.com/hyperledger/besu/pull/6163)
- New option `tx-pool-min-gas-price` to set a lower bound when accepting txs to the pool [#6098](https://github.com/hyperledger/besu/pull/6098)
- Update OpenJDK latest Docker image to use Java 21 [#6189](https://github.com/hyperledger/besu/pull/6189)
- Allow a transaction selection plugin to specify custom selection results [#6190](https://github.com/hyperledger/besu/pull/6190)
- Add `rpc-gas-cap` to allow users to set gas limit to the RPC methods used to simulate transactions[#6156](https://github.com/hyperledger/besu/pull/6156)
- Fix the unavailability of `address` field when returning an `Account` entity on GraphQL in case of unreachable world state [#6198](https://github.com/hyperledger/besu/pull/6198)
- Update OpenJ9 Docker image to latest version [#6226](https://github.com/hyperledger/besu/pull/6226)
- Add error messages on authentication failures with username and password [#6212](https://github.com/hyperledger/besu/pull/6212)
- Add `rocksdb usage` to the `storage` subcommand to allow users and dev to check columns families usage [#6185](https://github.com/hyperledger/besu/pull/6185)
- Ethereum Classic Spiral network upgrade [#6078](https://github.com/hyperledger/besu/pull/6078)

### Bug fixes
- Fix Docker image name clash between Besu and evmtool [#6194](https://github.com/hyperledger/besu/pull/6194)
- Fix `logIndex` in `eth_getTransactionReceipt` JSON RPC method [#6206](https://github.com/hyperledger/besu/pull/6206)

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.3/besu-23.10.3.zip / sha256 da7ef8a6ceb88d3e327cacddcdb32218d1750b464c14165a74068f6dc6e0871a
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.3/besu-23.10.3.tar.gz / sha256 73c834cf32c7bbe255d7d8cc7ca5d1eb0df8430b9114935c8dcf3a675b2acbc2

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.10.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-12-21 00:22:35 +0000 UTC
    </span>
</div>

