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
                ## 22.4.2

### Additions and Improvements
- Engine API Update: Replace deprecated INVALID_TERMINAL_BLOCK with INVALID last valid hash 0x0 [#3882](https://github.com/hyperledger/besu/pull/3882)
- Deprecate experimental merge flag and engine-rpc-enabled flag [#3875](https://github.com/hyperledger/besu/pull/3875)
- Update besu-native dependencies to 0.5.0 for linux arm64 support 
- Update ropsten TTD to 100000000000000000000000

### Bug Fixes
- Stop backward sync if genesis block has been reached [#3869](https://github.com/hyperledger/besu/pull/3869)
- Allow to backward sync to request headers back to last finalized block if present or genesis [#3888](https://github.com/hyperledger/besu/pull/3888)


### Download link
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.2/besu-22.4.2.zip
sha256: `e8e9eb7e3f544ecefeec863712fb8d3f6a569c9d70825a4ed2581c596db8fd45`
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.2/besu-22.4.2.tar.gz
sha256: `9db0c37440cb56bcf671b8de13e0ecb6235171a497bdad91020b8c4a9dac2a27`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.4.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-27 21:04:18 +0000 UTC
    </span>
</div>

