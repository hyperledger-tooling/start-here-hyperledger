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
                    22.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.4.0
                </span>
            </td>
            <td>
                ### Breaking Changes
- Version 22.4.x will be the last series to support Java 11. Version 22.7.0 will require Java 17 to build and run.
- In the Besu EVM Library all references to SHA3 have been renamed to the more accurate name Keccak256, including class names and comment. [#3749](https://github.com/hyperledger/besu/pull/3749)
- Removed the Gas object and replaced it with a primitive long [#3674](https://github.com/hyperledger/besu/pull/3674)

### Bug Fixes
- Fix nullpointer on snapsync [#3773](https://github.com/hyperledger/besu/pull/3773)
- Introduce RocksDbSegmentIdentifier to avoid changing the storage plugin [#3755](https://github.com/hyperledger/besu/pull/3755)

## Download Links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.0/besu-22.4.0.zip / SHA256 d89e102a1941e70be31c176a6dd65cd5f3d69c4c
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.0/besu-22.4.0.tar.gz / SHA256 868e38749dd40debe028624f8267f1fce7587010
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.4.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-04 05:45:08 +0000 UTC
    </span>
</div>

