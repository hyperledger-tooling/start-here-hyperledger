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
                    21.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.10.1
                </span>
            </td>
            <td>
                # Changelog

## 21.10.1

### Additions and Improvements
- Add CLI autocomplete scripts. [#2854](https://github.com/hyperledger/besu/pull/2854)
- Added support for PKCS11 keystore on PKI Block Creation. [#2865](https://github.com/hyperledger/besu/pull/2865)
- Optimize EVM Memory for MLOAD Operations [#2917](https://github.com/hyperledger/besu/pull/2917)
- Upgrade CircleCI OpenJDK docker image to version 11.0.12. [#2928](https://github.com/hyperledger/besu/pull/2928)
- Update JDK 11 to latest version in Besu Docker images. [#2925](https://github.com/hyperledger/besu/pull/2925)
- Add Sepolia proof-of-work testnet configurations [#2920](https://github.com/hyperledger/besu/pull/2920)
- Allow block period to be configured for IBFT2 and QBFT using transitions [\#2902](https://github.com/hyperledger/besu/pull/2902)
- Add support for binary messages (0x02) for websocket. [#2980](https://github.com/hyperledger/besu/pull/2980)

### Bug Fixes
- Do not change the sender balance, but set gas fee to zero, when simulating a transaction without enforcing balance checks. [#2454](https://github.com/hyperledger/besu/pull/2454)
- Ensure genesis block has the default base fee if london is at block 0 [#2920](https://github.com/hyperledger/besu/pull/2920) 
- Fixes the exit condition for loading a BonsaiPersistedWorldState for a sibling block of the last one persisted [#2967](https://github.com/hyperledger/besu/pull/2967)

### Early Access Features
- Enable plugins to expose custom JSON-RPC / WebSocket methods [#1317](https://github.com/hyperledger/besu/issues/1317)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/21.10.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-11-08 00:28:51 +0000 UTC
    </span>
</div>

