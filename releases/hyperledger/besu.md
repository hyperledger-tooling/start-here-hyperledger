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

The 22.7.3 release is predominantly focused on post-Merge fixes for Ethereum Mainnet and is strongly recommended for those users. It contains a variety of fixes and performance improvements that will alleviate issues for staking users around missed attestations and empty block proposals. This release also contains improvements for Besu's native crypto libraries to help with performance. It also fixes some RPC issues and provides a new flag --Xplugin-rocksdb-high-spec-enabled for higher spec'd hardware to increase database performance to speed up Besu in many operations (would recommend this for machines with 16GB of RAM or more). See the changelog for more.

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

### Download links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.3/besu-22.7.3.tar.gz / sha256: `b0863fe2406cab57caf8a02f2bf02632cc5198622ac48b69bc63c128703bbd79`
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.3/besu-22.7.3.zip / sha256: `368c6cb86119f8fe30bb12ab8c63b4d95a0fd8baf9c9414307a0a4033756b709`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.7.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-23 16:51:28 +0000 UTC
    </span>
</div>

