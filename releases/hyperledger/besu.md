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
                    22.10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.10.3
                </span>
            </td>
            <td>
                ## 22.10.3

### Breaking Changes
- Added `--rpc-max-logs-range` CLI option to allow limiting the number of blocks queried by `eth_getLogs` RPC API. Default value: 1000 [#4597](https://github.com/hyperledger/besu/pull/4597)
- The `graalvm` docker variant no longer meets the performance requirements for Ethereum Mainnet.  The `openjdk-11` and `openjdk-latest` variants are recommended in its place.

### Additions and Improvements
- Implement Eth/68 sub-protocol [#4715](https://github.com/hyperledger/besu/issues/4715)
- Increase the speed of modexp gas execution and execution. [#4780](https://github.com/hyperledger/besu/pull/4780)
- Added experimental CLI options `--Xeth-capability-max` and `--Xeth-capability-min` to specify a range of capabilities to be supported by the Eth protocol. [#4752](https://github.com/hyperledger/besu/pull/4752)
- Set the default curve in the EVMTool, like is done in production operations [#4790](https://github.com/hyperledger/besu/pull/4790)

### Bug Fixes
- Fix storage key format for eth_getProof so that it follows the EIP-1474 spec [#4564](https://github.com/hyperledger/besu/pull/4564)

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.10.3/besu-22.10.3.tar.gz / sha256: 7213f9445a84a196e94ae1877c6fdb1e51d37bfb19615da02ef5121d4f40e38c
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.10.3/besu-22.10.3.zip / sha256: 0bf6bc98e01b0c1045f1b7d841a390c575bc5203c2a4e543d922fbc1ea0d3d5d
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.10.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-12-09 21:45:34 +0000 UTC
    </span>
</div>

