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
                    22.4.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.4.0-RC2
                </span>
            </td>
            <td>
                ## 22.4.0-RC2

### Breaking Changes
- In the Besu EVM Library all references to SHA3 have been renamed to the more accurate name Kecack256, including class names and comment. [#3749](https://github.com/hyperledger/besu/pull/3749)

### Additions and Improvements
- Onchain node permissioning 
  - Log the enodeURL that was previously only throwing an IllegalStateException during the isPermitted check [#3697](https://github.com/hyperledger/besu/pull/3697),
  - Fail startup if node permissioning smart contract version does not match [#3765](https://github.com/hyperledger/besu/pull/3765)
- \[EXPERIMENTAL\] Add snapsync `--sync-mode="X_SNAP"` (only as client) [#3710](https://github.com/hyperledger/besu/pull/3710)
- Adapt Fast sync, and Snap sync, to use finalized block, from consensus layer, as pivot after the Merge [#3506](https://github.com/hyperledger/besu/issues/3506)
- Add IPC JSON-RPC interface (BSD/MacOS and Linux only) [#3695](https://github.com/hyperledger/besu/pull/3695)

## Download Links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.0-RC2/besu-22.4.0-RC2.zip /  SHA256 481eb77b0877e367029125dacee7ccfc3f64adcf24c2a7828612a2587b59c350
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.0-RC2/besu-22.4.0-RC2.tar.gz / SHA256 b4b109c1188721edb7625fdd404044f75ef9de9105a9f5499764c57bd560128d


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.4.0-RC2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-28 09:21:55 +0000 UTC
    </span>
</div>

