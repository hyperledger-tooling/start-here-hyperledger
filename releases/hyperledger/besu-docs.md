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
                    23.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.1.2
                </span>
            </td>
            <td>
                ## 23.1.2
This update is a mainnet-compatible Shanghai/Capella upgrade and is recommended for all Mainnet users. This update contains a small number of overall improvements and fixes but a large refactor of Bonsai. We have heard your issues loud and clear with the storage format and have taken the time to craft a new architecture that keeps the benefits (low storage, lightweight nodes) without the tradeoffs (worldstate issues, exceptions processing transactions, broken databases). Expect more details on this in a forthcoming blog post. We have also continued our cleanup of backwards sync and RPC. 

### Breaking Changes

### Additions and Improvements
- Schedule Shanghai (Shapella) fork for Mainnet [#5230](https://github.com/hyperledger/besu/pull/5230)
- Increase default from 1000 to 5000 for `--rpc-max-logs-range` [#5209](https://github.com/hyperledger/besu/pull/5209)
- Bonsai-safe refactor [#5123](https://github.com/hyperledger/besu/pull/5123)
- Safe tracing [#5197](https://github.com/hyperledger/besu/pull/5197)

### Bug Fixes
- Persist backward sync status to support resuming across restarts [#5182](https://github.com/hyperledger/besu/pull/5182)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/23.1.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-03-08 19:35:23 +0000 UTC
    </span>
</div>

