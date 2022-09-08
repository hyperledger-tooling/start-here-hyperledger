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
                    22.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.2
                </span>
            </td>
            <td>
                ## 22.7.2
### Besu 22.7.2 is a recommended release for the Merge and Mainnet users. 22.7.1 remains Merge-ready. This release provides additional robustness before the Merge with some fixes and improvements in sync, peering, and logging.

### Additions and Improvements
- Better management of jemalloc presence/absence in startup script [#4237](https://github.com/hyperledger/besu/pull/4237)
- Retry mechanism when getting a broadcasted block fail on all peers [#4271](https://github.com/hyperledger/besu/pull/4271)
- Filter out disconnected peers when fetching available peers [#4269](https://github.com/hyperledger/besu/pull/4269)
- Updated the default value of fast-sync-min-peers post merge [#4298](https://github.com/hyperledger/besu/pull/4298)
- Log imported block info post merge [#4310](https://github.com/hyperledger/besu/pull/4310)
- Pandas! Pandas now appear in 3 phases: The black bear and polar bear that are preparing? Those will appear when
your client has TTD configured (which is setup by default for mainnet), is in sync, and processing Proof of Work blocks. In the second phase you will see them powering up when the Terminal Total Difficulty block is added to the blockchain.
The final form of the Ethereum Panda will appear when the first finalized block is received from the Consensus Layer.

### Bug Fixes
- Accept wit/80 from Nethermind [#4279](https://github.com/hyperledger/besu/pull/4279)
- Properly shutdown the miner executor, to avoid waiting 30 seconds when stopping [#4353](https://github.com/hyperledger/besu/pull/4353)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.7.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-07 14:39:24 +0000 UTC
    </span>
</div>

