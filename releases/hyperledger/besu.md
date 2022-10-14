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
                    22.7.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.6
                </span>
            </td>
            <td>
                ## 22.7.6
Hotfix release of the 22.7.x series to address [#4495](https://github.com/hyperledger/besu/issues/4495) which could result in failed block proposals on merge networks. Besu version 22.7.6 will automatically invalidate the bloomfilter cache from prior versions of besu and regenerate the cache in the background.

### Additions and Improvements
- Bring GraphQL into compliance with execution-api specs [#4112](https://github.com/hyperledger/besu/pull/4112)

### Bug Fixes
- Corrects emission of blockadded events when rewinding during a re-org. [#4497](https://github.com/hyperledger/besu/issues/4497)

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.6/besu-22.7.6.zip / sha256: ae05040027b96ba458a08cfee8577dafe1d85a3afce793f00f798cedb3ab547d
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.6/besu-22.7.6.tar.gz / sha256: 9e538852f16fd39b884c4c342beaad813e33ab24890634c01eee3d37dc1da893

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.7.6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-10-07 23:19:08 +0000 UTC
    </span>
</div>

