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
                    21.10.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.10.0-RC1
                </span>
            </td>
            <td>
                # Changelog

## 21.10.0-RC1
### Additions and Improvements
- The EVM has been factored out into a standalone module, suitable for inclusion as a library. [#2790](https://github.com/hyperledger/besu/pull/2790)
- Low level performance improvements changes to cut worst-case EVM performance in half. [#2796](https://github.com/hyperledger/besu/pull/2796)
- Migrate `ExceptionalHaltReason` from an enum to an interface to allow downstream users of the EVM to add new exceptional halt reasons. [#2810](https://github.com/hyperledger/besu/pull/2810)
- reduces need for JUMPDEST analysis via caching [#2607](https://github.com/hyperledger/besu/pull/2821)
- Add support for custom private key file for public-key export and public-key export-address commands [#2801](https://github.com/hyperledger/besu/pull/2801)


### Bug Fixes
- Allow BESU_CONFIG_FILE environment to specify TOML file [#2455](https://github.com/hyperledger/besu/issues/2455)
- Fix bug with private contracts not able to call public contracts that call public contracts [#2816](https://github.com/hyperledger/besu/pull/2816)

### Early Access Features

### Download
https://hyperledger.jfrog.io/native/besu-binaries/besu/21.10.0-RC1/besu-21.10.0-RC1.zip \
SHA256: 536612e5e4d7a5e7a582f729f01ba591ba68cc389e8379fea3571ed85322ff51

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/21.10.0-RC1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-10-04 17:50:40 +0000 UTC
    </span>
</div>

