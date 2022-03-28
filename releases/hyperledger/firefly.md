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
                    v0.14.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.14.1
                </span>
            </td>
            <td>
                ## What's Changed
* Switch from https to ffdx by @gabriel-indik in https://github.com/hyperledger/firefly/pull/590
* [fetchreferences2] Adding event enrichment for all event types by @eberger727 in https://github.com/hyperledger/firefly/pull/623
* Re-read configuration on restart of orchestrator by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/624
* Add pool config to activate call by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/626
* [ui-v0.6.3] v0.6.3 release of ui in manifest by @eberger727 in https://github.com/hyperledger/firefly/pull/629
* Do not return an error from status if node lookup fails by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/630
* Update batch manager dispatch to track inflight and fix private blobs by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/633
* Created timestamp index on events shouldn't be unique by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/634
* [ui-v0.6.6] manifest release by @eberger727 in https://github.com/hyperledger/firefly/pull/635
* [ui-v0.6.7] ui manifest by @eberger727 in https://github.com/hyperledger/firefly/pull/636

![image](https://user-images.githubusercontent.com/6660217/160465588-3b4147cd-a59e-45e6-9088-d60fd2b2163e.png)


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.14.0...v0.14.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.14.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-28 18:43:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.14.0
                </span>
            </td>
            <td>
                ## Summary
* Major UI Update - Includes Activity, Blockchain, Off-Chain, Tokens, Network Map, and My Node sections (https://github.com/hyperledger/firefly-ui)
* [Custom contract APIs complete](https://hyperledger.github.io/firefly/gettingstarted/custom_contracts.html)
* [Enhanced subscription filters](https://hyperledger.github.io/firefly/gettingstarted/events.html)
* Event API enrichment
* Performance updates
* Bug fixes

<img alt="firefly_explorer" src="https://user-images.githubusercontent.com/2530008/159557568-f8fee202-a98f-4065-ac9f-d5463a8f8769.png">

## Breaking Changes and Migrations
* [FIR-9](https://github.com/hyperledger/firefly-fir/pull/9) Enhanced Identity API - custom identities and DID support
    * New namespaced API endpoints to manage identities within a namespace:
        * `POST` `/api/v1/namespaces/identities` - async broadcast, with `confirm=true` option for sync
        * `GET` `/api/v1/namespaces/identities` - collection of identities within namespace
        * `GET` `/api/v1/namespaces/identities/{iid}` - individual identity
        * `GET` `/api/v1/namespaces/identities/{iid}/did` - generated DID document
        * `GET` `/api/v1/namespaces/identities/{iid}/verifiers` - collection of keys
    * New non-namespaced endpoint is provided to look up identities by DID:
        * `GET` `/api/v1/network/identities/{did}` - efficient cached DID to identity resolution
    * Minor changes to existing APIs
        * `GET` `/api/v1/network/organizations` - now returns `identity` object
        * `GET` `/api/v1/network/nodes` - now returns `identity` object
        * `GET` `/api/v1/status` - now returns the `did` of the local organization
        * The `identity` field in nodes/orgs has been removed (used to contain the signing key)
        * The `did` field from `identity` is newly available on nodes and orgs
    * Existing node and organization identities are migrated to the new identity API
        * No migration support for non-root organizations, as the FIR-9 security model requires a verification transaction from the parent organization that is not available.
        * Existing root `organization` and `node` objects are migrated
        * New nodes joining a network can process previously published `organization` and `node` identities
        * All organizations now represented as an `identity` in the `ff_system` namespace with special types `org` and `node`
* Operation type strings have been updated for consistency:
    * `blockchain_pin_batch` - previously `blockchain_batch_pin`
    * `dataexchange_send_batch` - previously `dataexchange_batch_send`
    * `dataexchange_send_blob` - previously `dataexchange_blob_send`
    * `sharedstorage_upload_batch` - previously `sharedstorage_batch_broadcast`
    * `sharedstorage_upload_blob` - new
    * `sharedstorage_download_batch` - new
    * `sharedstorage_download_blob` - new
* Blockchain events
  * The `/api/v1/contracts/subscriptions` endpoint has been renamed to `/api/v1/contracts/listeners`
  * The `/messages/{msgid}/operations` endpoint has been removed
  * Events of type `blockchain_event` are now type `blockchain_event_received`
* The Ethereum plugin now expects a different input format to generate a FireFly Contract Interface from an Ethereum ABI. Please see the [docs for full details](https://hyperledger.github.io/firefly/gettingstarted/custom_contracts.html#request).
* The Public Storage plugin interface has been renamed to Shared Storage. The FireFly core config should be updated to replace `publicstorage` with `sharedstorage` as a root key. This release of FireFly is still backwards compatible with the old config key. 

## Updated Dependencies
* firefly-ethconnect [v3.1.5](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.5)
* firefly-fabconnect [v0.9.13](https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.13)
* firefly-tokens-erc1155 [v0.10.6](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v0.10.6)
* firefly-tokens-erc20-erc721 [v0.2.0](https://github.com/hyperledger/firefly-tokens-erc20-erc721/releases/tag/v0.2.0)
* firefly-ui [v0.6.0](https://github.com/hyperledger/firefly-ui/releases/tag/v0.6.0)


## What's Changed
* FIR-9: Identity enhancements by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/549
* Rename contract subscriptions to contract listeners by @nguyer in https://github.com/hyperledger/firefly/pull/548
* Rename Public Storage to Shared storage by @nguyer in https://github.com/hyperledger/firefly/pull/538
* Add missing itype column in SQLite migration by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/577
* Add Operations Manager, wrap all operations, and add retry functionality by @awrichar in https://github.com/hyperledger/firefly/pull/517
* Handle operations with retries in transaction status by @awrichar in https://github.com/hyperledger/firefly/pull/578
* [charts-by-type] histogram broken down by type by @eberger727 in https://github.com/hyperledger/firefly/pull/547
* Enhance subscription filters & event enrichment by @shorsher in https://github.com/hyperledger/firefly/pull/579
* add `fetchreferences` param to events api by @shorsher in https://github.com/hyperledger/firefly/pull/587
* Use CLI to deploy test contract by @nguyer in https://github.com/hyperledger/firefly/pull/589
* Update batch logic to only store+hash the manifest by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/582
* Batching message writer routines, to use multi-value insert across API calls on message/data insert by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/592
* Event lookup cache by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/593
* Add DB tuning to keep conns option, and correct cache bypass on group lookup by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/594
* Scope subscription check to the appropriate stream ID by @jebonfig in https://github.com/hyperledger/firefly/pull/591
* Move blob publish to broadcast batch dispatch, ensure public refs on inbound by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/596
* Performance enhancements from flame graph analysis by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/599
* Remove route /messages/{msgid}/operations by @awrichar in https://github.com/hyperledger/firefly/pull/602
* Upgrade dependencies by @nguyer in https://github.com/hyperledger/firefly/pull/605
* Add "info" field to token pools, consume "symbol" from connectors by @awrichar in https://github.com/hyperledger/firefly/pull/606
* [blockchainevents-charts] support for blockchain event charting by @eberger727 in https://github.com/hyperledger/firefly/pull/612
* Add E2E test support for ERC20/ERC721 by @awrichar in https://github.com/hyperledger/firefly/pull/611
* Add firstEvent field to contract listeners by @nguyer in https://github.com/hyperledger/firefly/pull/603
* Dependency updates for v0.14 testing by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/613
* Batch confirm messages, and update events to contain topic+tag by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/600
* Change node/org lookups to support name or ID by @awrichar in https://github.com/hyperledger/firefly/pull/616
* Update microservices versions for v0.14.0 by @nguyer in https://github.com/hyperledger/firefly/pull/615
* Restart stack and re-run E2E tests in daily integration job by @nguyer in https://github.com/hyperledger/firefly/pull/608
* Add Shared Storage Download Manager by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/607
* Add route to lookup identity by DID by @awrichar in https://github.com/hyperledger/firefly/pull/617
* Blockchain metrics for Ethereum by @nguyer in https://github.com/hyperledger/firefly/pull/584
* [ui-v0.6.0] PR for new UI release by @eberger727 in https://github.com/hyperledger/firefly/pull/619
* Custom contracts docs by @nguyer in https://github.com/hyperledger/firefly/pull/604
* [ui-v0.6.0-release] new ui release by @eberger727 in https://github.com/hyperledger/firefly/pull/620


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.13.1...v0.14.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-22 17:31:35 +0000 UTC
    </span>
</div>

