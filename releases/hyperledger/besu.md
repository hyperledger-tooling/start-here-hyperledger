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
                    24.5.2-RC0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.5.2-RC0
                </span>
            </td>
            <td>
                ### Additions and Improvements
- Remove deprecated Goerli testnet [#7049](https://github.com/hyperledger/besu/pull/7049)
- Default bonsai to use full-flat db and code-storage-by-code-hash [#6984](https://github.com/hyperledger/besu/pull/6894)
- New RPC methods miner_setExtraData and miner_getExtraData [#7078](https://github.com/hyperledger/besu/pull/7078)
- Disconnect peers that have multiple discovery ports since they give us bad neighbours [#7089](https://github.com/hyperledger/besu/pull/7089)

### Bug fixes
- Fix parsing `gasLimit` parameter when its value is > `Long.MAX_VALUE` [#7116](https://github.com/hyperledger/besu/pull/7116)
- Skip validation of withdrawals when importing BFT blocks since withdrawals don't apply to BFT chains [#7115](https://github.com/hyperledger/besu/pull/7115)

## New Contributors
* @knowmost made their first contribution in https://github.com/hyperledger/besu/pull/7005
* @seanyoung made their first contribution in https://github.com/hyperledger/besu/pull/7054

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.5.1...24.5.2-RC0
c3a702915556fdea16968c0924783d939f50863b561d27e565fe9ae9e0edd815  besu-24.5.2-RC0.tar.gz
2100ff8764d3cfa85aa259467d537bbc9fa08259e3036b8deb7e68eaf8e54dd8  besu-24.5.2-RC0.zip

`docker pull docker.io/hyperledger/besu:24.5.2-RC0`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.5.2-RC0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-05-17 01:54:19 +0000 UTC
    </span>
</div>

