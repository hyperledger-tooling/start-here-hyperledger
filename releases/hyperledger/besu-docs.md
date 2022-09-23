---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.3
                </span>
            </td>
            <td>
                ## 22.7.3

### Additions and Improvements
- Allow free gas networks in the London fee market [#4061](https://github.com/hyperledger/besu/issues/4061)
- Upgrade besu-native to 0.6.0 and use Blake2bf native implementation if available by default [#4264](https://github.com/hyperledger/besu/pull/4264)
- Resets engine QoS timer with every call to the engine API instead of only when ExchangeTransitionConfiguration is called [#4411](https://github.com/hyperledger/besu/issues/4411)
- ExchangeTransitionConfiguration mismatch will only submit a debug log not a warning anymore [#4411](https://github.com/hyperledger/besu/issues/4411)
- Upgrade besu-native to 0.6.1 and include linux arm64 build of bls12-381 [#4416](https://github.com/hyperledger/besu/pull/4416)
- Create a new flag on RocksDB (_--Xplugin-rocksdb-high-spec-enabled_) for high spec hardware to boost performance
- Transaction pool improvements to avoid filling the pool with not executable transactions, that could result in empty or semi-empty block proposals [#4425](https://github.com/hyperledger/besu/pull/4425) 
- Limit Transaction pool consumption by sender to a configurable percentage of the pool size [#4417](https://github.com/hyperledger/besu/pull/4417)

### Bug Fixes
- Retry block creation if there is a transient error and we still have time, to mitigate empty block issue [#4407](https://github.com/hyperledger/besu/pull/4407)
- Fix StacklessClosedChannelException in Besu and resulted timeout errors in CL clients ([#4398](https://github.com/hyperledger/besu/issues/4398), [#4400](https://github.com/hyperledger/besu/issues/4400))
- Return JSON-RPC error code instead of INVALID in engine api when certain storage exceptions are encountered ([#4349](https://github.com/hyperledger/besu/issues/4349))

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.7.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-21 14:06:54 +0000 UTC
    </span>
</div>

