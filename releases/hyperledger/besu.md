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
                    22.7.4 - Memory Leak Fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.4
                </span>
            </td>
            <td>
                ## 22.7.4

This is a STRONGLY RECOMMENDED upgrade which resolves known issues in the prior release (22.7.3). This version fixes a memory leak which was uncovered by fixes in 22.7.3.

### Bug Fixes
- Remove records that track transactions by sender when they are empty to same memory in the transaction pool [#4415](https://github.com/hyperledger/besu/pull/4415)
- Add Toml configuration file support for _--Xplugin-rocksdb-high-spec-enabled_ flag [#4438](https://github.com/hyperledger/besu/pull/4438)

### Download Links
[https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.4/besu-22.7.4.zip](https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.4/besu-22.7.4.zip) / sha256: `4f2a0c20bee7f266ec1dcb45fa90ae1ca42f4b22e9b21a601b7705357259aea9`
[https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.4/besu-22.7.4.tar.gz](https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.4/besu-22.7.4.tar.gz) / sha256: `a60efc4d515ac94710bbc6d61a24f409b03fcfc02323bee2a2d75c883fc99dce`
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.7.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-26 16:28:26 +0000 UTC
    </span>
</div>

