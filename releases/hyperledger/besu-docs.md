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
                    23.1.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.1.0-RC1
                </span>
            </td>
            <td>
                ## 23.1.0-RC1

### Breaking Changes
- Default configurations for the deprecated Ropsten, Kiln, Shandong, and Astor networks have been removed from the CLI network list. These networks can currently be accessed but will require a user-provided genesis configuration. [#4869](https://github.com/hyperledger/besu/pull/4869)

### Additions and Improvements

- Improve SLOAD and SSTORE performance by caching empty slots [#4874](https://github.com/hyperledger/besu/pull/4874)
- RPC methods that lookup block by hash will now return an error response if no block found [#4582](https://github.com/hyperledger/besu/pull/4582)
- Added support for `safe` and `finalized` strings for the RPC methods using defaultBlock parameter [#4902](https://github.com/hyperledger/besu/pull/4902)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/23.1.0-RC1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-01-11 22:24:46 +0000 UTC
    </span>
</div>

