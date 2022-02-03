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
                    v0.12.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.12.0
                </span>
            </td>
            <td>
                ## Summary
This is a large release as we come closer to the 1.0.0 milestone. All users are recommended to upgrade to this release when possible, taking into account all breaking API changes noted here.

Breaking API changes:
* All APIs deprecated in v0.11.0 or earlier are removed - see detailed [migration notes](https://github.com/hyperledger/firefly/wiki/Removed-APIs-in-v0.12.0)
* [Richer query parameters](https://github.com/hyperledger/firefly-fir/pull/4) for filtering collections - with breaking changes to the `^` operator

Other major items included in this release:
* Preview of [custom on-chain logic](https://github.com/hyperledger/firefly-fir/pull/2)
  * Provides flexible methods for interacting with your own contracts, deployed to the blockchain of your choice
  * New APIs are available under `/namespaces/{ns}/contracts` and`/namespaces/{ns}/apis`
  * Not yet guaranteed to be stable, and API is subject to change
* Support for new [ERC20 / ERC721](https://github.com/hyperledger/firefly-tokens-erc20-erc721) connector
* Overhaul of [Transaction type](https://github.com/hyperledger/firefly-fir/pull/8), and new BlockchainEvent type
* Support for [delivery confirmations](https://github.com/hyperledger/firefly-fir/pull/7) via DX plugin
* Support for more flexible signing via new config pointing at an [external address resolver](https://github.com/hyperledger/firefly/pull/436)
* First-class support for blob filenames on Data objects
* UI enhancements
  * Improved support for navigating and downloading file blobs
  * Filtering for token screens (pools, transfers, accounts)
* Bug fixes and improvements

## Updated Dependencies

* firefly-ethconnect [v3.1.2](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.2)
* firefly-fabconnect [v0.9.7](https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.7)
* firefly-dataexchange-https [v0.10.3](https://github.com/hyperledger/firefly-dataexchange-https/releases/tag/v0.10.3)
* firefly-tokens-erc1155 [v0.10.4](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v0.10.4)
* firefly-tokens-erc20-erc721 [v0.1.4](https://github.com/hyperledger/firefly-tokens-erc20-erc721/releases/tag/v0.1.4)
* firefly-ui [v0.5.0](https://github.com/hyperledger/firefly-ui/compare/v0.4.3...v0.5.0)

## What's Changed
* Fixing Websocket Connections when Prometheus Metrics Enabled by @hfuss in https://github.com/hyperledger/firefly/pull/371
* Set fetch-depth to get the full history in GitHub Actions by @nguyer in https://github.com/hyperledger/firefly/pull/377
* Fetch full history on all GitHub Actions by @nguyer in https://github.com/hyperledger/firefly/pull/378
* [helm] Publishing Helm Chart to GHCR via OCI by @hfuss in https://github.com/hyperledger/firefly/pull/359
* [psql-maxconns] default connection limit for postgresql by @eberger727 in https://github.com/hyperledger/firefly/pull/385
* Allow any company name in license header by @nguyer in https://github.com/hyperledger/firefly/pull/379
* Prevent send/receive deadlock in wsclient by @awrichar in https://github.com/hyperledger/firefly/pull/387
* API changes for Blob Friendly Names by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/381
* Fix unit test for wsclient send failure by @awrichar in https://github.com/hyperledger/firefly/pull/388
* Fixing Duplicate Metrics Registration when Unsetting preInit by @hfuss in https://github.com/hyperledger/firefly/pull/389
* Have DB creation script account for username by @drewmarshburn in https://github.com/hyperledger/firefly/pull/375
* Add Performance Testing Details to README by @eberger727 in https://github.com/hyperledger/firefly/pull/373
* Add postgres migrations for onchain-logic by @nguyer in https://github.com/hyperledger/firefly/pull/390
* FIR-4 (rich query updates) and FIR-7 (DX manifests) integration to onchain-logic branch by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/403
* Rectify Transactions and BlockchainEvents by @awrichar in https://github.com/hyperledger/firefly/pull/408
* Build the URL without the firefly port if it was omitted from stack.json by @jebonfig in https://github.com/hyperledger/firefly/pull/411
* Collapse onchain-logic into main by @awrichar in https://github.com/hyperledger/firefly/pull/410
* [erc20-payload] pass name and symbol to CreateTokenPool() by @eberger727 in https://github.com/hyperledger/firefly/pull/413
* Removing Helm Chart and Related CI Workflow by @hfuss in https://github.com/hyperledger/firefly/pull/412
* Update containerd by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/414
* PostgreSQL updates following merging of onchain-logic branch by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/417
* Fix token account listing on Postgres by @awrichar in https://github.com/hyperledger/firefly/pull/422
* Fix intermittent Fabric E2E test failure by @nguyer in https://github.com/hyperledger/firefly/pull/424
* Add ping/pong heartbeating to WSClient, and fix concurrent map on config by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/420
* Fail transaction when token transfer operation fails by @awrichar in https://github.com/hyperledger/firefly/pull/435
* Ready state changes require a bump to the message to re-sequence it by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/438
* JSON Schema validation for FFIs by @nguyer in https://github.com/hyperledger/firefly/pull/419
* Restore Transaction reference on TokenTransfer by @awrichar in https://github.com/hyperledger/firefly/pull/444
* Create a Transaction and Operation for contract invoke requests by @awrichar in https://github.com/hyperledger/firefly/pull/441
* Rename /contracts/events to /blockchainevents by @awrichar in https://github.com/hyperledger/firefly/pull/443
* Add convenience URL /transactions/{txnid}/blockchainevents by @awrichar in https://github.com/hyperledger/firefly/pull/446
* Allow calling JSONObject() on nil JSONAny by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/456
* Add Blockchain Transaction IDs to FireFly Transaction objects and add blockchain IDs to events by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/448
* Fixing E2E Tests for Multi-Member Networks by @hfuss in https://github.com/hyperledger/firefly/pull/459
* Avoid potential double-close of channels due to reconnects after tests complete by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/458
* Add route for /transactions/{txnid}/status by @awrichar in https://github.com/hyperledger/firefly/pull/457
* Add AddressResolver to Ethereum for key-to-address mapping by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/436
* Allow synchronous 200 response for token pool creation by @awrichar in https://github.com/hyperledger/firefly/pull/460
* Remove deprecated APIs by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/452
* ui version 0.5.0 by @shorsher in https://github.com/hyperledger/firefly/pull/464
* Add DefinitionBatchActions to execute after a batch of system definitions by @awrichar in https://github.com/hyperledger/firefly/pull/462
* Use /firefly prefix on local docs dev by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/461
* Allow passing a tokenIndex to "mint" by @awrichar in https://github.com/hyperledger/firefly/pull/465
* [v0.12.0-manifests] manifests for v0.12.0 by @eberger727 in https://github.com/hyperledger/firefly/pull/466

## New Contributors
* @drewmarshburn made their first contribution in https://github.com/hyperledger/firefly/pull/375

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.11.4...v0.12.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.12.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-02-02 22:04:41 +0000 UTC
    </span>
</div>

