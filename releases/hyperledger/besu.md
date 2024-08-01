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
                    24.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.7.1
                </span>
            </td>
            <td>
                ### Breaking Changes
- Remove deprecated sync modes (X_SNAP and X_CHECKPOINT). Use SNAP and CHECKPOINT instead [#7309](https://github.com/hyperledger/besu/pull/7309)
- Remove PKI-backed QBFT (deprecated in 24.5.1) Other forms of QBFT remain unchanged. [#7293](https://github.com/hyperledger/besu/pull/7293)
- Do not maintain connections to PoA bootnodes [#7358](https://github.com/hyperledger/besu/pull/7358). See [#7314](https://github.com/hyperledger/besu/pull/7314) for recommended alternative behaviour.

### Upcoming Breaking Changes
- Receipt compaction will be enabled by default in a future version of Besu. After this change it will not be possible to downgrade to the previous Besu version.
- --Xbonsai-limit-trie-logs-enabled is deprecated, use --bonsai-limit-trie-logs-enabled instead
- --Xbonsai-trie-logs-pruning-window-size is deprecated, use --bonsai-trie-logs-pruning-window-size instead
- `besu storage x-trie-log` subcommand is deprecated, use `besu storage trie-log` instead

### Additions and Improvements
- `--Xsnapsync-bft-enabled` option enables experimental support for snap sync with IBFT/QBFT permissioned Bonsai-DB chains [#7140](https://github.com/hyperledger/besu/pull/7140)
- Add support to load external profiles using `--profile` [#7265](https://github.com/hyperledger/besu/issues/7265)
- `privacy-nonce-always-increments` option enables private transactions to always increment the nonce, even if the transaction is invalid [#6593](https://github.com/hyperledger/besu/pull/6593)
- Added `block-test` subcommand to the evmtool which runs blockchain reference tests [#7293](https://github.com/hyperledger/besu/pull/7293)
- removed PKI backed QBFT [#7310](https://github.com/hyperledger/besu/pull/7310)
- Implement gnark-crypto for eip-2537 [#7316](https://github.com/hyperledger/besu/pull/7316)
- Improve blob size transaction selector [#7312](https://github.com/hyperledger/besu/pull/7312)
- Added EIP-7702 [#7237](https://github.com/hyperledger/besu/pull/7237)
- Implement gnark-crypto for eip-196 [#7262](https://github.com/hyperledger/besu/pull/7262)
- Add trie log pruner metrics [#7352](https://github.com/hyperledger/besu/pull/7352)
- Force bonsai-limit-trie-logs-enabled=false when sync-mode=FULL instead of startup error [#7357](https://github.com/hyperledger/besu/pull/7357)
- `--Xbonsai-parallel-tx-processing-enabled` option enables executing transactions in parallel during block processing for Bonsai nodes
- Reduce default trie log pruning window size from 30,000 to 5,000 [#7365](https://github.com/hyperledger/besu/pull/7365)
- Add option `--poa-discovery-retry-bootnodes` for PoA networks to always use bootnodes during peer refresh, not just on first start [#7314](https://github.com/hyperledger/besu/pull/7314)

### Bug fixes
- Fix `eth_call` deserialization to correctly ignore unknown fields in the transaction object. [#7323](https://github.com/hyperledger/besu/pull/7323)
- Prevent Besu from starting up with sync-mode=FULL and bonsai-limit-trie-logs-enabled=true for private networks [#7357](https://github.com/hyperledger/besu/pull/7357)
- Add 30 second timeout to trie log pruner preload [#7365](https://github.com/hyperledger/besu/pull/7365)
- Avoid executing pruner preload during trie log subcommands [#7366](https://github.com/hyperledger/besu/pull/7366)

### Release Artifacts
59ac352a86fd887225737a5fe4dad1742347edd3c3fbed98b079177e4ea8d544  besu-24.7.1.tar.gz
e616f8100f026a71a146a33847b40257c279b38085b17bb991df045cccb6f832  besu-24.7.1.zip

`docker pull docker.io/hyperledger/besu:24.7.1`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.7.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-26 02:17:08 +0000 UTC
    </span>
</div>

