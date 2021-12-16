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
                    22.1.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.0-RC1
                </span>
            </td>
            <td>
                ## 22.1.0-RC1

### 22.1.0-RC1 Breaking Changes
- Plugin API: BlockHeader.getBaseFee() method now returns an optional Wei instead of an optional Long [#3065](https://github.com/hyperledger/besu/issues/3065)

### Additions and Improvements
- Represent baseFee as Wei instead of long accordingly to the spec [#2785](https://github.com/hyperledger/besu/issues/2785)
- Adding support of the NO_COLOR environment variable as described in the [NO_COLOR](https://no-color.org/) standard [#3085](https://github.com/hyperledger/besu/pull/3085)
- Add `privx_findFlexiblePrivacyGroup` RPC Method, `privx_findOnchainPrivacyGroup` will be removed in a future release [#3075](https://github.com/hyperledger/besu/pull/3075)
- The invalid value is now shown when `--bootnodes` cannot parse an item to make it easier to identify which option is invalid. 
- Adding two new options to be able to specify desired TLS protocol version and Java cipher suites [#3105](https://github.com/hyperledger/besu/pull/3105)
- Implements [EIP-4399](https://eips.ethereum.org/EIPS/eip-4399) to repurpose DIFFICULTY opcode after the merge as a source of entropy from the Beacon chain. [#3081](https://github.com/hyperledger/besu/issues/3081)

### Bug Fixes
- Change the base docker image from Debian Buster to Ubuntu 20.04 [#3171](https://github.com/hyperledger/besu/issues/3171) fixes [#3045](https://github.com/hyperledger/besu/issues/3045)
- Update log4j to 2.16.0.

### Early Access Features
- Add support for additional JWT authentication algorithms [#3017](https://github.com/hyperledger/besu/pull/3017)

### Download Links 
[besu-22.1.0-RC1.zip](https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC1/besu-22.1.0-RC1.zip) - 8f471a30a7d22a6830c5f7ed87d1f2110bdaeb6751007ffa0fb44783a7c80850
[besu-22.1.0-RC1.tar.gz](https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC1/besu-22.1.0-RC1.tar.gz) - 302ead51c85bf282047104974968ce88ce626df609082700e6e187b26180e0fd
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.1.0-RC1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-15 21:08:54 +0000 UTC
    </span>
</div>

