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
                    23.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.1.1
                </span>
            </td>
            <td>
                ## 23.1.1 Goerli Shanghai/Capella Release
This update is required for the Goerli Shanghai/Capella upgrade and recommended for all Mainnet users. If you use Besu on Goerli, update to 23.1.1. If you previously used 23.1.1-RC1, update to test 23.1.1 on Goerli. 

### Breaking Changes

### Additions and Improvements
- Add support for Shanghai in Sepolia https://github.com/hyperledger/besu/pull/5088
- Add implementation for engine_getPayloadBodiesByRangeV1 and engine_getPayloadBodiesByHashV1 https://github.com/hyperledger/besu/pull/4980
- If a PoS block creation repetition takes less than a configurable duration, then waits before next repetition https://github.com/hyperledger/besu/pull/5048
- Allow other users to read the /opt/besu dir when using docker https://github.com/hyperledger/besu/pull/5092
- Invalid params - add some error detail #5066
- Added the option --kzg-trusted-setup to pass a custom setup file for custom networks or to override the default one for named networks [#5084](https://github.com/hyperledger/besu/pull/5084)
- Gas accounting for EIP-4844 [#4992](https://github.com/hyperledger/besu/pull/4992)
- Goerli configs for shapella [#5151](https://github.com/hyperledger/besu/pull/5151)

### Bug Fixes
- Fix engine_getPayloadV2 block value calculation https://github.com/hyperledger/besu/issues/5040
- Moves check for init code length before balance check https://github.com/hyperledger/besu/pull/5077
- Address post-shanghai sync issue [#5714](https://github.com/hyperledger/besu/pull/5174)
- Address concurrency problems with eth_call [#5179](https://github.com/hyperledger/besu/pull/5179)

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.1/besu-23.1.1.tar.gz / sha256: 11c3e5cdbc06df16a690e7ee9f98eefa46848f9fa280824b6e4c896d88f6b975
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.1.1/besu-23.1.1.zip / sha256: afcf852f193adb8e82d187aa4f02e4669f12cc680270624d37101b94cf37adec

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.1.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-03-07 22:13:44 +0000 UTC
    </span>
</div>

