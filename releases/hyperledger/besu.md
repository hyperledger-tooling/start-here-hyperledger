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
                    22.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.4.4
                </span>
            </td>
            <td>
                ## 22.4.4

This release resolves known issues in 22.4.3 with respect to snap-sync and state root mismatch/worldstate unavailable issues.  Certain configurations may still experience excessive off-heap memory consumption by rocksdb, which will be addressed by a future release in the 22.7.x series.

### Additions and Improvements

- Do not require a minimum block height when downloading headers or blocks [#3911](https://github.com/hyperledger/besu/pull/3911)
- When on PoS the head can be only be updated by ForkchoiceUpdate [#3994](https://github.com/hyperledger/besu/pull/3994)
- Add TTD and DNS to Sepolia config [#4024](https://github.com/hyperledger/besu/pull/4024)

### Bug Fixes
- Fixed a snapsync issue that can sometimes block the healing step [#3920](https://github.com/hyperledger/besu/pull/3920)
- remove peer block height requirements for block fetching [#3911](https://github.com/hyperledger/besu/pull/3911)
- allow upgrade whether websockets enabled or not [#4019](https://github.com/hyperledger/besu/pull/4019)
- jwt auth on websockets [#4039](https://github.com/hyperledger/besu/pull/4039)
- Fixed a state root mismatch issue on bonsai that may appear occasionally [#4041](https://github.com/hyperledger/besu/pull/4041)
- Fixed a trie log layer issue on bonsai during reorg [#4069](https://github.com/hyperledger/besu/pull/4069)

Download links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.4/besu-22.4.4.tar.gz
sha256: e7cfb082f6d7985e760fa2cd1e18c266777fafb48137d2a9c3b68ec3f6d2a732
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.4.4/besu-22.4.4.zip
sha256: 84a7bee8fc35c78fd6d9e7bbdc5cd28c577d95487480bb03b9642a3111b71bc3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.4.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-07-08 15:56:45 +0000 UTC
    </span>
</div>

