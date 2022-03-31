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
                    22.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.3
                </span>
            </td>
            <td>
                ### Breaking Changes
- Remove the experimental flag for bonsai tries CLI options `--data-storage-format` and `--bonsai-maximum-back-layers-to-load` [#3578](https://github.com/hyperledger/besu/pull/3578)

### Deprecations
- `--tx-pool-hashes-max-size` is now deprecated and has no more effect and it will be removed in a future release.

### Additions and Improvements
- Tune transaction synchronization parameter to adapt to mainnet traffic [#3610](https://github.com/hyperledger/besu/pull/3610)
- Improve eth/66 support [#3616](https://github.com/hyperledger/besu/pull/3616)
- Avoid reprocessing remote transactions already seen [#3626](https://github.com/hyperledger/besu/pull/3626)
- Upgraded jackson-databind dependency version [#3647](https://github.com/hyperledger/besu/pull/3647)

## Download Links
 - https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.3/besu-22.1.3.zip /  SHA256 9dafb80f2ec9ce8d732fd9e9894ca2455dd02418971c89cd6ccee94c53354d5d

 - https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.3/besu-22.1.3.tar.gz / SHA256 f9f8d37353aa4b5d12e87c08dd86328c1cffc591c6fc9e076c0f85a1d4663dfe
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.1.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-30 17:17:35 +0000 UTC
    </span>
</div>

