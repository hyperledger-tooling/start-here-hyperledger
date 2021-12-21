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
                    v0.11.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.11.3
                </span>
            </td>
            <td>
                ## Summary
- Dependency updates and bug fixes
- Helm/Kubernetes deployment template updated for fabric and prometheus metrics

## Updated Dependencies
* firefly-ethconnect [v3.1.0](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.0)
* firefly-fabconnect [v0.9.3](https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.3)
* firefly-tokens-erc1155 [v0.10.2](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v0.10.2)
* firefly-dataexchange-https [v0.9.3](https://github.com/hyperledger/firefly-dataexchange-https/releases/tag/v0.9.3)

## What's Changed
* Fabric connector needs to subscribe from zero by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/361
* Support configuration keys when the value type is a list by @jebonfig in https://github.com/hyperledger/firefly/pull/362
* [helm] Adding Storage for DX Blobs and PVC Templating Improvements by @hfuss in https://github.com/hyperledger/firefly/pull/354
* Fix send-to-self for private messages, and add group query URLs by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/363
* [helm] Support for Prometheus Metrics by @hfuss in https://github.com/hyperledger/firefly/pull/338
* [fabric] Dockerfile for Compiling firefly-go for Linux by @hfuss in https://github.com/hyperledger/firefly/pull/357
* Update manifest ready for v0.11.3 release by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/364
* [helm] Fabconnect Support by @hfuss in https://github.com/hyperledger/firefly/pull/356

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.11.2...v0.11.3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.11.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-21 03:41:51 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.11.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.11.2
                </span>
            </td>
            <td>
                ## Summary
This patch release includes important fixes and hardening for recent features. Major highlights:
* New charts UI and UI fixes for token panels
* Handling for token connectors that don't guarantee a unique URI for each NFT

## Updated Dependencies
* firefly-dataexchange-https [v0.9.3](https://github.com/hyperledger/firefly-dataexchange-https/releases/tag/v0.9.3)
* firefly-ui [v0.4.3](https://github.com/hyperledger/firefly-ui/compare/v0.4.2...v0.4.3)

## What's Changed
* Fix Hyperledger Image Refs and Migration Job's Postgres URL in Helm Chart by @hfuss in https://github.com/hyperledger/firefly/pull/340
* Fix image repos by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/288
* Updates to handle recursive structures in swagger - depends on kin-openapi change by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/337
* Return an empty slice (rather than nil) for zero token accounts by @awrichar in https://github.com/hyperledger/firefly/pull/346
* Address coverage drop from #337 by @awrichar in https://github.com/hyperledger/firefly/pull/347
* on transfer/mint/burn fail, set transaction & operation as failed by @shorsher in https://github.com/hyperledger/firefly/pull/351
* update prometheus client version by @shorsher in https://github.com/hyperledger/firefly/pull/352
* Replace UpsertOperation with InsertOperation by @awrichar in https://github.com/hyperledger/firefly/pull/350
* Metrics endpoint to support charting by @eberger727 in https://github.com/hyperledger/firefly/pull/341
* Remove unique index on token URIs by @awrichar in https://github.com/hyperledger/firefly/pull/353
* Reduce overhead of gocritic by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/344
* ui version 0.4.3 by @shorsher in https://github.com/hyperledger/firefly/pull/358
* Update manifest for dataexchange-https by @awrichar in https://github.com/hyperledger/firefly/pull/360


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.11.1...v0.11.2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.11.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-14 18:05:30 +0000 UTC
    </span>
</div>

