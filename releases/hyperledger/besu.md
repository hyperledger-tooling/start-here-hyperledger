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
                    23.1.1-RC1 - Sepolia Shanghai Release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.1.1-RC1
                </span>
            </td>
            <td>
                ## Sepolia Shanghai Release aka Sepolia Shapella aka Shapolia

This update is **not recommended for mainnet users**.

Besu 23.1.1-RC1 is a **required update for Sepolia users**

Sepolia Shanghai hardfork scheduled for: **Tue Feb 28 2023 04:04:48 UTC**

---

This release has everything from [23.1.0](https://github.com/hyperledger/besu/releases/tag/23.1.0) and in addition the following:

### Additions and Improvements
* Add support for Shanghai in Sepolia https://github.com/hyperledger/besu/pull/5088
* Add implementation for engine_getPayloadBodiesByRangeV1 and engine_getPayloadBodiesByHashV1 https://github.com/hyperledger/besu/pull/4980
* If a PoS block creation repetition takes less than a configurable duration, then waits before next repetition https://github.com/hyperledger/besu/pull/5048
* Allow other users to read the /opt/besu dir when using docker https://github.com/hyperledger/besu/pull/5092
* Invalid params - add some error detail #5066

### Bug fixes
* Fix engine_getPayloadV2 block value calculation https://github.com/hyperledger/besu/issues/5040
* Moves check for init code length before balance check https://github.com/hyperledger/besu/pull/5077

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.1-RC1/besu-23.1.1-RC1.tar.gz / sha256: 82cff41f3eace02006b0e670605848e0e77e045892f8fa9aad66cbd84a88221e

https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.1-RC1/besu-23.1.1-RC1.zip / sha256: 469c8d6a8ca9d78ee111ff1128d00bf3bcddacbf5b800ef6047717a2da0cc21d
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.1.1-RC1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-02-20 01:58:04 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    23.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.1.0
                </span>
            </td>
            <td>
                ## 23.1.0
Besu 23.1.0 is a recommended update for Mainnet users. Thank you all for your patience as we crafted this quarterly release.

This is a rather large release with some breaking changes, so please be sure to read these notes carefully before you upgrade any Besu instances. We are including a move to Java 17 LTS. To build and run Besu, please make sure you have Java 17 on the host machine. Additionally, there are a host of spec compliance changes that change existing formats, so please check the specific RPC updates. Lastly, this release formalizes a deprecation notice for GoQuorum privacy modes and IBFT1.0 in Besu. These will be removed in the 23.4 series, unless otherwise stated.

From the improvements and fixes side, we have a host of execution performance improvements and fixes for defects with bonsai storage. We have also included an error detection and auto-heal capability for nodes that encounter state issues. This should keep nodes online and validating that may have previously required a resync.

One final note. 23.1.0 is not a Shanghai ready release. If you intend to test Besu on the long-lived testnets like Zhejiang, please [follow the instructions here](https://notes.ethereum.org/@launchpad/zhejiang). We will have more to share on our official Shanghai releases soon.

### Breaking Changes
- Change JsonRpc http service to return the error -32602 (Invalid params) with a 200 http status code
- Besu requires minimum Java 17 and up to build and run [#3320](https://github.com/hyperledger/besu/issues/3320)
- PKCS11 with nss module (PKCS11 based HSM can be used in DevP2P TLS and QBFT PKI) does not work with RSA keys
in Java 17. SoftHSM is tested manually and working. (Other PKCS11 HSM are not tested). The relevant unit and acceptance
tests are updated to use EC private keys instead of RSA keys.
- Change eth_feeHistory parameter `blockCount` to accept hexadecimal string (was accepting plain integer) [#5047](https://github.com/hyperledger/besu/pull/5047)
- Default configurations for the deprecated Ropsten, Kiln, Shandong, and Astor networks have been removed from the CLI network list. These networks can currently be accessed but will require a user-provided genesis configuration. [#4869](https://github.com/hyperledger/besu/pull/4869)
- GoQuorum-compatible privacy is deprecated and will be removed in 23.4
- IBFT 1.0 is deprecated and will be removed in 23.4
- Optimize SSTORE Operation execution time (memoize current and original value) [#4836](https://github.com/hyperledger/besu/pull/4836)

### Additions and Improvements
- Default rpc batch request to 1024 [#5104](https://github.com/hyperledger/besu/pull/5104) [#5108](https://github.com/hyperledger/besu/pull/5108)
- Add a new CLI option to limit the number of requests in a single RPC batch request. [#4965](https://github.com/hyperledger/besu/pull/4965)
- Support for new DATAHASH opcode as part of EIP-4844 [#4823](https://github.com/hyperledger/besu/issues/4823)
- Send only hash announcement for blob transaction type [#4940](https://github.com/hyperledger/besu/pull/4940)
- Add `excess_data_gas` field to block header [#4958](https://github.com/hyperledger/besu/pull/4958)
- Add `max_fee_per_data_gas` field to transaction [#4970](https://github.com/hyperledger/besu/pull/4970)
- Added option to evm CLI tool to allow code execution at specific forks [#4913](https://github.com/hyperledger/besu/pull/4913)
- Improve get account performance by using the world state updater cache [#4897](https://github.com/hyperledger/besu/pull/4897)
- Add new KZG precompile and option to override the trusted setup being used [#4822](https://github.com/hyperledger/besu/issues/4822)
- Add implementation for eth_createAccessList RPC method [#4942](https://github.com/hyperledger/besu/pull/4942)
- Updated reference tests to v11.3 [#4996](https://github.com/hyperledger/besu/pull/4996)
- Add DebugGetRawBlock and DebugGetRawHeader RPC methods [#5011](https://github.com/hyperledger/besu/pull/5011)
- Besu requires minimum Java 17 and up to build and run [#3320](https://github.com/hyperledger/besu/issues/3320)
- Add worldstate auto-heal mechanism [#5059](https://github.com/hyperledger/besu/pull/5059)
- Support for EIP-4895 - Withdrawals for Shanghai fork
- Improve SLOAD and SSTORE performance by caching empty slots [#4874](https://github.com/hyperledger/besu/pull/4874)
- RPC methods that lookup block by hash will now return an error response if no block found [#4582](https://github.com/hyperledger/besu/pull/4582)
- Added support for `safe` and `finalized` strings for the RPC methods using defaultBlock parameter [#4902](https://github.com/hyperledger/besu/pull/4902)
- Added post-execution state logging option to EVM Tool [#4709](https://github.com/hyperledger/besu/pull/4709)
- Add access list to Transaction Call Object [#4802](https://github.com/hyperledger/besu/issues/4801)
- Add timestamp fork support, including shanghaiTime and cancunTime forks [#4743](https://github.com/hyperledger/besu/pull/4743)
- Optimization:  Memoize transaction size and hash at the same time [#4812](https://github.com/hyperledger/besu/pull/4812)
- Add chain data pruning feature with three experimental CLI options: `--Xchain-pruning-enabled`, `--Xchain-pruning-blocks-retained` and `--Xchain-pruning-frequency` [#4686](https://github.com/hyperledger/besu/pull/4686)
  - Note that chain pruning is hidden and disabled by default. Once you choose to enable chain pruning, a new column family will be added to the db and you cannot roll back to a previous versi
on of Besu.

### Bug Fixes
- Mitigation fix for stale bonsai code storage leading to log rolling issues on contract recreates [#4906](https://github.com/hyperledger/besu/pull/4906)
- Ensure latest cached layered worldstate is subscribed to storage, fix problem with RPC calls using 'latest' [#5076](https://github.com/hyperledger/besu/pull/5076)
- Fix for segmentation faults on worldstate truncation, snap-sync starts [#4786](https://github.com/hyperledger/besu/pull/4786)
- Fix for worldstate mismatch on failed forkchoiceUpdate [#4862](https://github.com/hyperledger/besu/pull/4862)

Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.0/besu-23.1.0.tar.gz / sha256: 9081da04d47c3ff0a6ecc2256d353c7a02212f9b46f2c867a9365e18026c3a6e
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.0/besu-23.1.0.zip / sha256: e037f5c8f976150af40403311d1c81018f4c3dfbef0ad33324d8c3e708d1fdca
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-02-17 01:32:32 +0000 UTC
    </span>
</div>

