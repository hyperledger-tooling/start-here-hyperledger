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
                    21.10.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.10.0-RC2
                </span>
            </td>
            <td>
                # Changelog

## 21.10.0-RC2
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
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/21.10.0-RC2/besu-21.10.0-RC2.zip \
SHA256: 4a279b515a2525ae42299ba74518a109444776b01c501ee4d96ea345c35194eb

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/21.10.0-RC2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-10-12 07:05:58 +0000 UTC
    </span>
</div>

