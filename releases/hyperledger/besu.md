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
                    22.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.4.1
                </span>
            </td>
            <td>
                ### Additions and Improvements
- GraphQL - allow null log topics in queries which match any topic [#3662](https://github.com/hyperledger/besu/pull/3662)
- multi-arch docker builds for amd64 and arm64 [#2954](https://github.com/hyperledger/besu/pull/2954)
- Filter Netty native lib errors likewise the pure Java implementation [#3807](https://github.com/hyperledger/besu/pull/3807)
- Add ropsten terminal total difficulty config [#3871](https://github.com/hyperledger/besu/pull/3871)

### Bug Fixes
- Stop the BlockPropagationManager when it receives the TTD reached event [#3809](https://github.com/hyperledger/besu/pull/3809)
- Correct getMixHashOrPrevRandao to return the value present in the block header [#3839](https://github.com/hyperledger/besu/pull/3839)

## Download Links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.1/besu-22.4.1.zip / SHA256 076f688900ca515f13774c22d64d6a7ddc6351f24c0e7db823d304c84f9a0a2e
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.1/besu-22.4.1.tar.gz / SHA256 7910bcbb1d09ad9e872441f3a3a371755949be210df7b7eb3948b6fe850f374e
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.4.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-20 06:38:58 +0000 UTC
    </span>
</div>

