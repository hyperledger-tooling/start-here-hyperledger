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
                    22.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.0
                </span>
            </td>
            <td>
                # Changelog

## 22.1.0

### Breaking Changes
- Plugin API: BlockHeader.getBaseFee() method now returns an optional Wei instead of an optional Long [#3065](https://github.com/hyperledger/besu/issues/3065)
- Removed deprecated hash variable `protected volatile Hash hash;` which was used for private transactions [#3110](https://github.com/hyperledger/besu/pull/3110)

### Additions and Improvements
- Add support for additional JWT authentication algorithms [#3017](https://github.com/hyperledger/besu/pull/3017)
- Represent baseFee as Wei instead of long accordingly to the spec [#2785](https://github.com/hyperledger/besu/issues/2785)
- Implements [EIP-4399](https://eips.ethereum.org/EIPS/eip-4399) to repurpose DIFFICULTY opcode after the merge as a source of entropy from the Beacon chain. [#3081](https://github.com/hyperledger/besu/issues/3081)
- Re-order external services (e.g JsonRpcHttpService) to start before blocks start processing [#3118](https://github.com/hyperledger/besu/pull/3118)
- Stream JSON RPC responses to avoid creating big JSON strings in memory [#3076](https://github.com/hyperledger/besu/pull/3076)
- Ethereum Classic Mystique Hard Fork [#3256](https://github.com/hyperledger/besu/pull/3256)
- Genesis file parameter `blockperiodseconds` is validated as a positive integer on startup to prevent unexpected runtime behaviour [#3186](https://github.com/hyperledger/besu/pull/3186)
- Add option to require replay protection for locally submitted transactions [\#1975](https://github.com/hyperledger/besu/issues/1975)
- Update to block header validation for IBFT and QBFT to support London fork EIP-1559 [#3251](https://github.com/hyperledger/besu/pull/3251)
- Move into SLF4J as logging facade [#3285](https://github.com/hyperledger/besu/pull/3285)
- Changing the order in which we traverse the word state tree during fast sync. This should improve fast sync during subsequent pivot changes.
- Updated besu-native to version 0.4.3 [#3331](https://github.com/hyperledger/besu/pull/3331)
- Refactor synchronizer to asynchronously retrieve blocks from peers, and to change peer when retrying to get a block. [#3326](https://github.com/hyperledger/besu/pull/3326)
- Disable RocksDB TTL compactions [#3356](https://github.com/hyperledger/besu/pull/3356)
- add a websocket frame size configuration CLI parameter [3368][https://github.com/hyperledger/besu/pull/3379]
- Add `--ec-curve` parameter to export/export-address public-key subcommands [#3333](https://github.com/hyperledger/besu/pull/3333)

### Bug Fixes
- Change the base docker image from Debian Buster to Ubuntu 20.04 [#3171](https://github.com/hyperledger/besu/issues/3171) fixes [#3045](https://github.com/hyperledger/besu/issues/3045)
- Make 'to' field optional in eth_call method according to the spec [#3177](https://github.com/hyperledger/besu/pull/3177)
- Update to log4j 2.17.1. Resolves potential vulnerability only exploitable when using custom log4j configurations that are writable by untrusted users.
- Fix regression on cors-origin star value
- Fix for ethFeeHistory accepting hex values for blockCount
- Fix a sync issue, when the chain downloader incorrectly shutdown when a task in the pipeline is cancelled. [#3319](https://github.com/hyperledger/besu/pull/3319)
- add a websocket frame size configuration CLI parameter [3368][https://github.com/hyperledger/besu/pull/3379]
- Prevent node from peering to itself [#3342](https://github.com/hyperledger/besu/pull/3342)
- Fix an `IndexOutOfBoundsException` exception when getting block from peers. [#3304](https://github.com/hyperledger/besu/issues/3304)
- Handle legacy eth64 without throwing null pointer exceptions [#3343](https://github.com/hyperledger/besu/pull/3343)

### Download Links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0/besu-22.1.0.tar.gz \ SHA256 232bd7f274691ca14c26289fdc289d3fcdf69426dd96e2fa1601f4d079645c2f
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0/besu-22.1.0.zip \ SHA256 1b701ff5b647b64aff3d73d6f1fe3fdf73f14adbe31504011eff1660ab56ad2b

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-02-15 20:09:46 +0000 UTC
    </span>
</div>

