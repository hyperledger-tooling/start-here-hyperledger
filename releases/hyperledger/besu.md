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
                    23.1.0-beta
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.1.0-BETA
                </span>
            </td>
            <td>
                ## 23.1.0-beta

### Breaking Changes
- GoQuorum-compatible privacy is deprecated and will be removed in 23.4
- IBFT 1.0 is deprecated and will be removed in 23.4
- Optimize SSTORE Operation execution time (memoize current and original value) [#4836](https://github.com/hyperledger/besu/pull/4836)

### Additions and Improvements
- Added post-execution state logging option to EVM Tool [#4709](https://github.com/hyperledger/besu/pull/4709)
- Add access list to Transaction Call Object [#4802](https://github.com/hyperledger/besu/issues/4801)
- Add timestamp fork support, including shanghaiTime and cancunTime forks [#4743](https://github.com/hyperledger/besu/pull/4743)
- Optimization:  Memoize transaction size and hash at the same time [#4812](https://github.com/hyperledger/besu/pull/4812)

### Bug Fixes
- Fix for segmentation faults on worldstate truncation, snap-sync starts [#4786](https://github.com/hyperledger/besu/pull/4786)
- Fix for worldstate mismatch on failed forkchoiceUpdate [#4862](https://github.com/hyperledger/besu/pull/4862)

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.0-beta/besu-23.1.0-beta.tar.gz / sha256: ab25ee41d9464216fa2a8bbf5a788b0963e383b505c5d664c63ac96efe5ef657
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.0-beta/besu-23.1.0-beta.zip / sha256: 250d87736ae09408394e584f99f1e15b5e30769d87a4eec777eca2bbb81882df
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.1.0-BETA" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-12-23 21:47:43 +0000 UTC
    </span>
</div>

