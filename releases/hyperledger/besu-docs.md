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
                    22.4.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.4.2
                </span>
            </td>
            <td>
                ### Additions and Improvements
- Engine API Update: Replace deprecated INVALID_TERMINAL_BLOCK with INVALID last valid hash 0x0 https://github.com/hyperledger/besu/pull/3882
- Deprecate experimental merge flag and engine-rpc-enabled flag https://github.com/hyperledger/besu/pull/3875
- update besu-native dependencies to 0.5.0 for linux arm64 support

### Bug Fixes
- Stop backward sync if genesis block has been reached https://github.com/hyperledger/besu/pull/3869
- Allow to backward sync to request headers back to last finalized block if present or genesis https://github.com/hyperledger/besu/pull/3888
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.4.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-26 20:34:57 +0000 UTC
    </span>
</div>

