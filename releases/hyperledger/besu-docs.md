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
                21.10.0-RC2
## Additions and Improvements
* The EVM has been factored out into a standalone module, suitable for inclusion as a library. #2790
* Low level performance improvements changes to cut worst-case EVM performance in half. #2796
* Migrate ExceptionalHaltReason from an enum to an interface to allow downstream users of the EVM to add new exceptional halt reasons. #2810
* reduces need for JUMPDEST analysis via caching #2607
* Add support for custom private key file for public-key export and public-key export-address commands #2801
## Bug Fixes
* Allow BESU_CONFIG_FILE environment to specify TOML file #2455
* Fix bug with private contracts not able to call public contracts that call public contracts #2816
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/21.10.0-RC2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-10-12 06:44:05 +0000 UTC
    </span>
</div>

