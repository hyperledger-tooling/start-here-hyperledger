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
                    23.1.1-RC1 - Sepolia Shanghai Release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.1.1-RC1
                </span>
            </td>
            <td>
                ## Sepolia Shanghai Release aka Sepolia Shapella aka Shapolia

This update is **not recommended for mainnet users**.

Besu 23.1.1-RC1 is a **required update for Sepolia users**

Sepolia Shanghai hardfork scheduled for: **Tue Feb 28 2023 04:04:48 UTC**

---

This release has everything from [23.1.0](https://github.com/hyperledger/besu/releases/tag/23.1.0) and in addition the following:

### Additions and Improvements
* Add support for Shanghai in Sepolia https://github.com/hyperledger/besu/pull/5088
* Add implementation for engine_getPayloadBodiesByRangeV1 and engine_getPayloadBodiesByHashV1 https://github.com/hyperledger/besu/pull/4980
* If a PoS block creation repetition takes less than a configurable duration, then waits before next repetition https://github.com/hyperledger/besu/pull/5048
* Allow other users to read the /opt/besu dir when using docker https://github.com/hyperledger/besu/pull/5092
* Invalid params - add some error detail #5066

### Bug fixes
* Fix engine_getPayloadV2 block value calculation https://github.com/hyperledger/besu/issues/5040
* Moves check for init code length before balance check https://github.com/hyperledger/besu/pull/5077

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.1-RC1/besu-23.1.1-RC1.tar.gz / sha256: 82cff41f3eace02006b0e670605848e0e77e045892f8fa9aad66cbd84a88221e

https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.1-RC1/besu-23.1.1-RC1.zip / sha256: 469c8d6a8ca9d78ee111ff1128d00bf3bcddacbf5b800ef6047717a2da0cc21d
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.1.1-RC1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-02-20 01:58:04 +0000 UTC
    </span>
</div>

