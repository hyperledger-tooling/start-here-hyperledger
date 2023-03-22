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

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.2/besu-23.1.2.tar.gz / sha256: 3d3a709a3aab993a0801b412a4719d74e319f942ddc13fb0f30b3c4a54d12538
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.2/besu-23.1.2.zip / sha256: 2a9ff091cb4349fc23625a52089400bb6529a831eb22d15d0221cb27039ab203

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.1.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-03-18 03:56:07 +0000 UTC
    </span>
</div>

