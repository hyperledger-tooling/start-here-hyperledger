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
                    24.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.5.4
                </span>
            </td>
            <td>
                The same as [24.5.2](https://github.com/hyperledger/besu/releases/tag/24.5.2) with the only change being to fix the inability to build from source.

### Bug fixes
- Rectify build from source failure with updated 0.8.4 artifacts from besu-native [#7210](https://github.com/hyperledger/besu/pull/7210) 
2d2082bd2ebebdc24a45007dd3c9c45ea9b430ef8a4b6025be4ef3376317f5d7  besu-24.5.4.tar.gz
9d8774a69f90986477aabd2d7713ed22df1e2f29ed6b62a1889ac21675026f83  besu-24.5.4.zip

`docker pull docker.io/hyperledger/besu:24.5.4`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.5.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-12 06:07:06 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.6.0
                </span>
            </td>
            <td>
                ### Breaking Changes
- Java 21 has been enforced as minimum version to build and run Besu.
- With --bonsai-limit-trie-logs-enabled by default in this release, historic trie log data will be removed from the database unless sync-mode=FULL. It respects the --bonsai-historical-block-limit setting so shouldn't break any RPCs, but may be breaking if you are accessing this data from the database directly. Can be disabled with --bonsai-limit-trie-logs-enabled=false
- In profile=ENTERPRISE, use sync-mode=FULL (instead of FAST) and data-storage-format=FOREST (instead of BONSAI) [#7186](https://github.com/hyperledger/besu/pull/7186)
  - If this breaks your node, you can reset sync-mode=FAST and data-storage-format=BONSAI

### Upcoming Breaking Changes
- Receipt compaction will be enabled by default in a future version of Besu. After this change it will not be possible to downgrade to the previous Besu version.
- PKI-backed QBFT will be removed in a future version of Besu. Other forms of QBFT will remain unchanged.
- --Xbonsai-limit-trie-logs-enabled is deprecated, use --bonsai-limit-trie-logs-enabled instead
- --Xbonsai-trie-logs-pruning-window-size is deprecated, use --bonsai-trie-logs-pruning-window-size instead
- Receipt compaction will be enabled by default in a future version of Besu. After this change it will not be possible to downgrade to the previous Besu version.

### Additions and Improvements
- Add two counters to DefaultBlockchain in order to be able to calculate TPS and Mgas/s [#7105](https://github.com/hyperledger/besu/pull/7105)
- Enable --Xbonsai-limit-trie-logs-enabled by default, unless sync-mode=FULL [#7181](https://github.com/hyperledger/besu/pull/7181)
- Promote experimental --Xbonsai-limit-trie-logs-enabled to production-ready, --bonsai-limit-trie-logs-enabled [#7192](https://github.com/hyperledger/besu/pull/7192)
- Promote experimental --Xbonsai-trie-logs-pruning-window-size to production-ready, --bonsai-trie-logs-pruning-window-size [#7192](https://github.com/hyperledger/besu/pull/7192)
- `admin_nodeInfo` JSON/RPC call returns the currently active EVM version [#7127](https://github.com/hyperledger/besu/pull/7127)
- Improve the selection of the most profitable built block [#7174](https://github.com/hyperledger/besu/pull/7174)

### Bug fixes
- Make `eth_gasPrice` aware of the base fee market [#7102](https://github.com/hyperledger/besu/pull/7102)

fa86e5c6873718cd568e3326151ce06957a5e7546b52df79a831ea9e39b857ab  besu-24.6.0.tar.gz
8b2d3a674cd7ead68b9ca68fea21e46d5ec9b278bbadc73f8c13c6a1e1bc0e4d  besu-24.6.0.zip

`docker pull docker.io/hyperledger/besu:24.6.0`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.6.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-11 03:45:07 +0000 UTC
    </span>
</div>

