---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.11.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.11.1
                </span>
            </td>
            <td>
                ## Summary
This patch release includes important fixes and hardening for recent features. Major highlights:

- Fixed bugs with some token transfer events being ignored
- Added support for retrieving the URI attached to each non-fungible token
- Updated EthConnect release with significant new features, particularly when using Kafka
- Added initial prometheus metrics for batch pins

## Updated Dependencies
* firefly-ethconnect [v3.1.0](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.0)
* firefly-fabconnect [v0.9.2](https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.2)
* firefly-dataexchange-https [v0.9.2](https://github.com/hyperledger/firefly-dataexchange-https/releases/tag/v0.9.2)
* firefly-tokens-erc1155 [v0.10.1](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v0.10.1)
* firefly-ui [v0.4.2](https://github.com/hyperledger/firefly-ui/compare/v0.4.1...v0.4.2)

## What's Changed
* Update dependencies for v0.11.0 release by @nguyer in https://github.com/hyperledger/firefly/pull/333
* Remove "skipEventstreamInit" parameters by @awrichar in https://github.com/hyperledger/firefly/pull/329
* add batchpin counter prometheus metric by @shorsher in https://github.com/hyperledger/firefly/pull/334
* Add token URI by @awrichar in https://github.com/hyperledger/firefly/pull/335
* Split event stream helpers into separate files by @awrichar in https://github.com/hyperledger/firefly/pull/323
* Add "Getting Started" documentation for tokens by @awrichar in https://github.com/hyperledger/firefly/pull/306
* Move definitions of datatypes and tokens to their proper namespace by @nguyer in https://github.com/hyperledger/firefly/pull/312
* Leverage new token transfer id from plugin by @awrichar in https://github.com/hyperledger/firefly/pull/336
* bump ui to version 0.4.2 by @shorsher in https://github.com/hyperledger/firefly/pull/339
* Update dependencies for v0.11.1 release by @awrichar in https://github.com/hyperledger/firefly/pull/342

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.11.0...v0.11.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.11.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-01 16:28:13 +0000 UTC
    </span>
</div>

