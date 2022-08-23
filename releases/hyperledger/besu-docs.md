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
                    22.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.1
                </span>
            </td>
            <td>
                ## 22.7.1 - Mandatory Upgrade for The Merge on Ethereum Mainnet!

Hi folks! This is the big one... This update includes configurations that make Besu compatible with the Mainnet Merge! Make sure you read up on [the Merge here](https://besu.hyperledger.org/en/stable/Concepts/Merge/) to understand what is happening to both your node and the network ([and check out this page to make sure you are prepared](https://besu.hyperledger.org/en/latest/public-networks/how-to/prepare-for-the-merge/)). The date for the Merge is likely to be the 15th of September and can be tracked [here](https://bordel.wtf). 

Since Besu releases on a two-weekly cadence, we anticipate one more (likely optional) release prior to the Merge with last minute fixes, cleanup, and more so stay tuned for that. Make sure your nodes are in sync prior to the 15th if you want to participate in history! 

### Additions and Improvements
- Introduce a cap to reputation score increase [#4230](https://github.com/hyperledger/besu/pull/4230)
- Add experimental CLI option for `--Xp2p-peer-lower-bound` [#4200](https://github.com/hyperledger/besu/pull/4200)
- Improve pending blocks retrieval mechanism [#4227](https://github.com/hyperledger/besu/pull/4227)
- set mainnet terminal total difficulty [#4260](https://github.com/hyperledger/besu/pull/4260)

### Bug Fixes
- Fixes off-by-one error for mainnet TTD fallback [#4223](https://github.com/hyperledger/besu/pull/4223)
- Fix off-by-one error in AbstractRetryingPeerTask [#4254](https://github.com/hyperledger/besu/pull/4254)
- Refactor and fix retrying get block switching peer [#4256](https://github.com/hyperledger/besu/pull/4256)
- Fix encoding of key (short hex) in eth_getProof [#4261](https://github.com/hyperledger/besu/pull/4261)
- Fix for post-merge networks fast-sync [#4224](https://github.com/hyperledger/besu/pull/4224), [#4276](https://github.com/hyperledger/besu/pull/4276)

### Download links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.1/besu-22.7.1.tar.gz / sha256: `7cca4c11e1d7525c172f2af9fbf456d134ada60e970d8b6abcfcd6c623b5dd36`
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.1/besu-22.7.1.zip / sha256: `ba6e0b9b65ac36d041a5072392f119ff76e8e9f53a3d7b1e1a658ef1e4705d7a`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.7.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-08-19 17:31:22 +0000 UTC
    </span>
</div>

