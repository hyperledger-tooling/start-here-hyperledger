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
                    24.5.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.5.2
                </span>
            </td>
            <td>
                ### Additions and Improvements
- Remove deprecated Goerli testnet [#7049](https://github.com/hyperledger/besu/pull/7049)
- Default bonsai to use full-flat db and code-storage-by-code-hash [#6984](https://github.com/hyperledger/besu/pull/6894)
- New RPC methods miner_setExtraData and miner_getExtraData [#7078](https://github.com/hyperledger/besu/pull/7078)
- Disconnect peers that have multiple discovery ports since they give us bad neighbours [#7089](https://github.com/hyperledger/besu/pull/7089)

### Upcoming Breaking Changes
- Version 24.5.x will be the last series to support Java 17. Next release after versions 24.5.x will require Java 21 to build and run.
- Receipt compaction will be enabled by default in a future version of Besu. After this change it will not be possible to downgrade to the previous Besu version.
- PKI-backed QBFT will be removed in a future version of Besu. Other forms of QBFT will remain unchanged.

### Known Issues
- [Frequency: occasional < 10%] Chain download halt. Only affects new syncs (new nodes syncing from scratch). Symptom: Block import halts, despite having a full set of peers and world state downloading finishing. Generally restarting besu will resolve the issue. We are tracking this in [#6884](https://github.com/hyperledger/besu/pull/6884)

### Bug fixes
- Fix parsing `gasLimit` parameter when its value is > `Long.MAX_VALUE` [#7116](https://github.com/hyperledger/besu/pull/7116)
- Skip validation of withdrawals when importing BFT blocks since withdrawals don't apply to BFT chains [#7115](https://github.com/hyperledger/besu/pull/7115)

## New Contributors
* @knowmost made their first contribution in https://github.com/hyperledger/besu/pull/7005
* @seanyoung made their first contribution in https://github.com/hyperledger/besu/pull/7054

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.5.1...24.5.2


4049bf48022ae073065b46e27088399dfb22035e9134ed4ac2c86dd8c5b5fbe9  besu-24.5.2.tar.gz
23966b501a69e320e8f8f46a3d103ccca45b53f8fee35a6543bd9a260b5784ee  besu-24.5.2.zip

`docker pull docker.io/hyperledger/besu:24.5.2`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.5.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-27 01:48:13 +0000 UTC
    </span>
</div>

