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
                    21.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.10.0
                </span>
            </td>
            <td>
                # Changelog

## 21.10.0

### Additions and Improvements
- The EVM has been factored out into a standalone module, suitable for inclusion as a library. [#2790](https://github.com/hyperledger/besu/pull/2790)
- Low level performance improvements changes to cut worst-case EVM performance in half. [#2796](https://github.com/hyperledger/besu/pull/2796)
- Migrate `ExceptionalHaltReason` from an enum to an interface to allow downstream users of the EVM to add new exceptional halt reasons. [#2810](https://github.com/hyperledger/besu/pull/2810)
- reduces need for JUMPDEST analysis via caching [#2607](https://github.com/hyperledger/besu/pull/2821)
- Add support for custom private key file for public-key export and public-key export-address commands [#2801](https://github.com/hyperledger/besu/pull/2801)
- Add CLI autocomplete scripts. [#2854](https://github.com/hyperledger/besu/pull/2854)
- Added support for PKCS11 keystore on PKI Block Creation. [#2865](https://github.com/hyperledger/besu/pull/2865)
- add support for ArrowGlacier hardfork [#2943](https://github.com/hyperledger/besu/issues/2943)

### Bug Fixes
- Allow BESU_CONFIG_FILE environment to specify TOML file [#2455](https://github.com/hyperledger/besu/issues/2455)
- Fix bug with private contracts not able to call public contracts that call public contracts [#2816](https://github.com/hyperledger/besu/pull/2816)
- Fixes the exit condition for loading a BonsaiPersistedWorldState for a sibling block of the last one persisted [#2967](https://github.com/hyperledger/besu/pull/2967)
- Fixes bonsai getMutable regression affecting fast-sync [#2934](https://github.com/hyperledger/besu/pull/2934)
- Regression in RC1 involving LogOperation and frame memory overwrites [#2908](https://github.com/hyperledger/besu/pull/2908)
- Allow `eth_call` and `eth_estimateGas` to accept contract address as sender. [#2891](https://github.com/hyperledger/besu/pull/2891)

### Early Access Features
- Enable plugins to expose custom JSON-RPC / WebSocket methods [#1317](https://github.com/hyperledger/besu/issues/1317)

### Download Link
https://hyperledger.jfrog.io/native/besu-binaries/besu/21.10.0/besu-21.10.0.zip \
SHA256: 71374454753c2ee595f4f34dc6913f731818d50150accbc98088aace313c6935
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/21.10.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-11-01 22:48:10 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    21.10.0-RC4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.10.0-RC4
                </span>
            </td>
            <td>
                ## 21.10.0-RC4

### Additions and Improvements

### Bug Fixes
- Fixes the exit condition for loading a BonsaiPersistedWorldState for a sibling block of the last one persisted [#2967](https://github.com/hyperledger/besu/pull/2967)
- Fixes bonsai getMutable regression affecting fast-sync [#2934](https://github.com/hyperledger/besu/pull/2934)

### Early Access Features
### Download Link
https://hyperledger.jfrog.io/native/besu-binaries/besu/21.10.0-RC4/besu-21.10.0-RC4.zip \
SHA256: b16e15764b8bc06c5c3f9f19bc8b99fa48e7894aa5a6ccdad65da49bbf564793

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/21.10.0-RC4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-10-28 18:23:54 +0000 UTC
    </span>
</div>

