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
                    22.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.1
                </span>
            </td>
            <td>
                ### Additions and Improvements
- Allow optional RPC methods that bypass authentication [#3382](https://github.com/hyperledger/besu/pull/3382)
- Execution layer (The Merge):
  - Extend block creation and mining to support The Merge [#3412](https://github.com/hyperledger/besu/pull/3412)
  - Backward sync [#3410](https://github.com/hyperledger/besu/pull/3410)
  - Extend validateAndProcessBlock to return an error message in case of failure, so it can be returned to the caller of ExecutePayload API [#3411](https://github.com/hyperledger/besu/pull/3411)
  - Persist latest finalized block [#2913](https://github.com/hyperledger/besu/issues/2913)
  - Add PostMergeContext, and stop syncing after the swith to PoS [#3453](https://github.com/hyperledger/besu/pull/3453)
  - Add header validation rules needed to validate The Merge blocks [#3454](https://github.com/hyperledger/besu/pull/3454)
  - Add core components: controller builder, protocol scheduler, coordinator, block creator and processor. [#3461](https://github.com/hyperledger/besu/pull/3461)
  - Execution specific RPC endpoint [#2914](https://github.com/hyperledger/besu/issues/2914), [#3350](https://github.com/hyperledger/besu/pull/3350)
- QBFT consensus algorithm is production ready

## Download Links
 - https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.1/besu-22.1.1.zip /  SHA256 cfff79e19e5f9a184d0b62886990698b77d019a0745ea63b5f9373870518173e
 - https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.1/besu-22.1.1.tar.gz / SHA256 51cc9d35215f977ac7338e5c611c60f225fd6a8c1c26f188e661624a039e83f3

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.1.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-02-24 23:11:27 +0000 UTC
    </span>
</div>

