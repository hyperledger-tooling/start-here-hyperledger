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
                    21.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.7.1
                </span>
            </td>
            <td>
                ### Additions and Improvements

This release contains improvements and bugfixes for optimum compatibility with other London client versions.

- `priv_call` now uses NO_TRACING OperationTracer implementation which improves memory usage [\#2482](https://github.com/hyperledger/besu/pull/2482)
- Ping and Pong messages now support ENR encoding as scalars or bytes [\#2512](https://github.com/hyperledger/besu/pull/2512)

### Download Link
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/21.7.1/besu-21.7.1.zip
sha256 83fc44e39a710a95d8b6cbbbf04010dea76122bafcc633a993cd15304905a402
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/21.7.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-14 17:39:54 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    21.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.7.0
                </span>
            </td>
            <td>
                ## 21.7.0

### Additions and Improvements
This release contains the activation blocks for London across all supported testnets. They are: 
  * Ropsten 10_499_401 (24 Jun 2021)
  * Goerli 5_062_605 (30 Jun 2021)
  * Rinkeby 8_897_988 (7 Jul 2021)
  * Mainnet 12_965_000 (4 Aug 2021)
- eip-1559 changes: accept transactions which have maxFeePerGas below current baseFee [\#2374](https://github.com/hyperledger/besu/pull/2374)
- Introduced transitions for IBFT2 block rewards [\#1977](https://github.com/hyperledger/besu/pull/1977) 
- Change Ethstats's status from experimental feature to stable. [\#2405](https://github.com/hyperledger/besu/pull/2405) 
- Fixed disabling of native libraries for secp256k1 and altBn128. [\#2163](https://github.com/hyperledger/besu/pull/2163)
- eth_feeHistory API for wallet providers [\#2466](https://github.com/hyperledger/besu/pull/2466)

### Bug Fixes
- Ibft2 could create invalid RoundChange messages in some circumstances containing duplicate prepares [\#2449](https://github.com/hyperledger/besu/pull/2449)
- Updated `eth_sendRawTransaction` to return an error when maxPriorityFeePerGas exceeds maxFeePerGas [\#2424](https://github.com/hyperledger/besu/pull/2424)
- Fixed NoSuchElementException with EIP1559 transaction receipts when using eth_getTransactionReceipt [\#2477](https://github.com/hyperledger/besu/pull/2477)

### Early Access Features
- QBFT is a Byzantine Fault Tolerant consensus algorithm, building on the capabilities of IBFT and IBFT 2.0. It aims to provide performance improvements in cases of excess round change, and provides interoperability with other EEA compliant clients, such as GoQuorum.
  - Note: QBFT currently only supports new networks. Existing networks using IBFT2.0 cannot migrate to QBFT. This will become available in a future release.
  - Note: QBFT is an early access feature pending community feedback. Please make use of QBFT in new development networks and reach out in case of issues or concerns
- GoQuorum-compatible privacy. This mode uses Tessera and is interoperable with GoQuorum.
  - Note: GoQuorum-compatible privacy is an early access feature pending community feedback.

### Download Link
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/21.7.0/besu-21.7.0.zip
sha256 389465fdcc2cc5e5007a02dc2b8a2c43d577198867316bc5cc4392803ed71034
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/21.7.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-08 17:48:45 +0000 UTC
    </span>
</div>

