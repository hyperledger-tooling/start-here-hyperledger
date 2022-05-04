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
                    v1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0
                </span>
            </td>
            <td>
                ## Summary

Version 1.0.0 🎉

This release includes lots of major hardening, performance improvements, and bug fixes, as well as more complete documentation and OpenAPI specifications.

* Massive performance improvements across the board
* Up-to-date documentation and fully annotated OpenAPI specification
* Overhaul of UI
* Cleaner logs and error messages
* Lots of bug fixes and miscellaneous enhancements

You can view the release notes for each release candidate for more details: [rc.1](https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.1) [rc.2](https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.2) [rc.3](https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.3) [rc.4](https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.4) [rc.5](https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.5) [rc.6](https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.6)

## Breaking Changes and Migrations

* **firefly-dataexchange-https** must be upgraded to 1.0.0 alongside FireFly core, as the ack event [has been renamed](https://github.com/hyperledger/firefly/pull/656) from "commit" to "ack". Upgrading dependencies alongside FireFly is always recommended, but running mismatched versions of FireFly and dataexchange in this case will cause event processing to stall completely.
* Some of the APIs for creating contract listeners have changed - see #685
* Some field names under TokenPool, TokenTransfer, and TokenApproval have been adjusted - see #709

## Updated Dependencies

* firefly-ethconnect [v3.1.8](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.8)
* firefly-fabconnect [v0.9.14](https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.14)
* firefly-dataexchange-https [v1.0.0](https://github.com/hyperledger/firefly-dataexchange-https/releases/tag/v1.0.0)
* firefly-tokens-erc1155 [v1.0.0](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v1.0.0)
* firefly-tokens-erc20-erc721 [v1.0.0](https://github.com/hyperledger/firefly-tokens-erc20-erc721/releases/tag/v1.0.0)
* firefly-ui [v1.0.0](https://github.com/hyperledger/firefly-ui/releases/tag/v1.0.0)

## What's Changed
* Cache blockchain events for event enrichment by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/638
* Add index on message_id for token transfers by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/639
* Update txType in private message schema by @gabriel-indik in https://github.com/hyperledger/firefly/pull/637
* Fix `transactions_id` index by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/643
* Update our cache for event enrichment on message confirm by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/642
* Add extra convenience functions for identities by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/641
* Fix IF EXISTS check on transactions_id INDEX migration by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/645
* Call out memory needed in docs by @keeganhrobinson in https://github.com/hyperledger/firefly/pull/649
* Add background workers to flush updates to operations by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/646
* Use a single commit to generate all batch ops, before initiating the HTTP calls by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/647
* Assign nonces more efficiently, with minimal DB ops by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/650
* Change messages_data join table indexes for data_id lookup by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/653
* Cannot assume zero as reason to insert vs. update by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/652
* [charts-config] chart buckets are now capped at a configurable max by @eberger727 in https://github.com/hyperledger/firefly/pull/651
* [chart-test-fix] chart testing fix by @eberger727 in https://github.com/hyperledger/firefly/pull/655
* Move DX events interface to async with callback by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/656
* Avoid blocking event processing threads when queuing rewinds by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/657
* Proper handling of token approval events by @shorsher in https://github.com/hyperledger/firefly/pull/662
* Latest UI v0.6.9 by @hfuss in https://github.com/hyperledger/firefly/pull/667
* [charts-isCapped] adding isCapped key to charts response by @eberger727 in https://github.com/hyperledger/firefly/pull/669
* Remove misleading payload_ref DB field and fix Group JSON tag by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/666
* Add rewinder to handle enrichment off event poller critical path by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/665
* Refactor OpenAPI Spec generation by @nguyer in https://github.com/hyperledger/firefly/pull/658
* Remove references to old firefly-e2e stack name by @awrichar in https://github.com/hyperledger/firefly/pull/671
* Clean up blockchain parameters returned by token connectors by @awrichar in https://github.com/hyperledger/firefly/pull/673
* Check up-front for duplicate token pool name by @awrichar in https://github.com/hyperledger/firefly/pull/674
* Do not update cache until messages/data assured to be in DB by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/670
* [ui-v0.6.10] manifest by @eberger727 in https://github.com/hyperledger/firefly/pull/676
* Update manifest for v1.0.0-rc.1 by @nguyer in https://github.com/hyperledger/firefly/pull/677
* Configuration docs, and packaging config/i18n for re-use by microservices by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/678
* Fix make docker command in release build GitHub Action by @nguyer in https://github.com/hyperledger/firefly/pull/682
* Enforce config descriptions by @nguyer in https://github.com/hyperledger/firefly/pull/681
* Remove extra postgres migrations by @nguyer in https://github.com/hyperledger/firefly/pull/683
* Fix postgres migrations and add to PR checks by @nguyer in https://github.com/hyperledger/firefly/pull/690
* Add contract listeners only by event definition or event pathname by @awrichar in https://github.com/hyperledger/firefly/pull/685
* Rename "contract" field to "interface" on FFIMethod/FFIEvent by @awrichar in https://github.com/hyperledger/firefly/pull/691
* New operations admin APIs and revamped change-event listener on admin WebSocket by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/668
* Move ffresty to pkg for use by other microservices by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/688
* Make http server framework re-usable by microservices by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/697
* Add completed configuration descriptions and types by @nguyer in https://github.com/hyperledger/firefly/pull/695
* Status plugins by @eberger727 in https://github.com/hyperledger/firefly/pull/689
* Update ruby deps by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/698
* Include interface metadata routes in FFI-generated Swagger by @awrichar in https://github.com/hyperledger/firefly/pull/687
* Add /api/v1/status/websockets by @awrichar in https://github.com/hyperledger/firefly/pull/680
* [ui-v0.7.0] manifest and image by @eberger727 in https://github.com/hyperledger/firefly/pull/701
* Reject Contract API updates with an ID mismatch by @awrichar in https://github.com/hyperledger/firefly/pull/705
* Add helpers at /apis/{apiName}/listeners/{eventPath} by @awrichar in https://github.com/hyperledger/firefly/pull/696
* Readme and documentation updates by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/708
* Add descriptions for all API routes by @nguyer in https://github.com/hyperledger/firefly/pull/702
* Restore getting started section by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/712
* WebSocket disconnections should be info messages by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/714
* Add token provider to container logs name to make it unique by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/711
* Rename contract listener "protocol_id" to "backend_id" by @awrichar in https://github.com/hyperledger/firefly/pull/717
* Fix token approvals and clarify fields "protocolId", "locator", and "subject" by @awrichar in https://github.com/hyperledger/firefly/pull/709
* Move "special" operation update handling out of Operations Manager by @awrichar in https://github.com/hyperledger/firefly/pull/720
* DID rewind by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/716
* E2E account creation by @nguyer in https://github.com/hyperledger/firefly/pull/707
* OpenAPI cleanup items by @awrichar in https://github.com/hyperledger/firefly/pull/719
* Parse input params for /query endpoints in ffi2swagger by @awrichar in https://github.com/hyperledger/firefly/pull/724
* New Getting Started Guide by @nguyer in https://github.com/hyperledger/firefly/pull/721
* Fix image link in Sandbox docs by @nguyer in https://github.com/hyperledger/firefly/pull/727
* Fix account creation for nightly integration runs by @nguyer in https://github.com/hyperledger/firefly/pull/729
* Allow config suffix to be changed by microservices using config package by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/730
* Add "tx.blockchainId" to BlockchainEvent type by @awrichar in https://github.com/hyperledger/firefly/pull/725
* Accept "decimals" from token plugins on pool creation by @awrichar in https://github.com/hyperledger/firefly/pull/731
* Add event for failed token pool creation operations by @awrichar in https://github.com/hyperledger/firefly/pull/734
* Use blank type for JSONAny in OpenAPI by @awrichar in https://github.com/hyperledger/firefly/pull/733
* Honor "confirm" parameter for blockchain invoke by @awrichar in https://github.com/hyperledger/firefly/pull/722
* UI v0.7.1 by @eberger727 in https://github.com/hyperledger/firefly/pull/741
* Update dependencies for v1.0.0-rc.5 release by @nguyer in https://github.com/hyperledger/firefly/pull/742
* Resolve pool activation operations more cleanly by @awrichar in https://github.com/hyperledger/firefly/pull/746
* Remove server-side HTML sanitization of error messages by @awrichar in https://github.com/hyperledger/firefly/pull/752
* Rename docs pages for better hierarchy by @nguyer in https://github.com/hyperledger/firefly/pull/750
* Misc cleanup for contract listeners by @awrichar in https://github.com/hyperledger/firefly/pull/749
* Format JSON errors from connectors by @awrichar in https://github.com/hyperledger/firefly/pull/748
* Configurable JSON Formatter and Caller Reporting for Logs by @hfuss in https://github.com/hyperledger/firefly/pull/737
* Ensuring Senders Do Not Download Their Own Batches in Response to Pin Events by @hfuss in https://github.com/hyperledger/firefly/pull/745
* Token approvals should return empty array instead of nil by @awrichar in https://github.com/hyperledger/firefly/pull/759
* remove rocketchat from docs by @shorsher in https://github.com/hyperledger/firefly/pull/760
* Merge wsconfig to wsclient so microservices can use it by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/738
* Fill in blockchain TX ID for contract listener events by @awrichar in https://github.com/hyperledger/firefly/pull/762
* "decimals" is not a valid input by @awrichar in https://github.com/hyperledger/firefly/pull/766
* add additional event enrichment by @shorsher in https://github.com/hyperledger/firefly/pull/765
* Add change events to operations, by adding namespace to ResolveOperation by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/764
* Simplfy solc compilation of BatchPin contract by @nguyer in https://github.com/hyperledger/firefly/pull/627
* Add table name to debug on every SQL call by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/747
* Firefly E2E Test updates by @calbritt in https://github.com/hyperledger/firefly/pull/755
* Version Command by @hfuss in https://github.com/hyperledger/firefly/pull/763
* Omit "connector" from token transfer/approval inputs by @awrichar in https://github.com/hyperledger/firefly/pull/770
* Add prefix for signer by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/769
* Update architecture diagram to include OpenAPI generator and fix link by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/767
* [ui-v1.0.0] manifest by @eberger727 in https://github.com/hyperledger/firefly/pull/771
* Update manifest.json for v1.0.0 by @nguyer in https://github.com/hyperledger/firefly/pull/772
* Add E2E test for contract APIs and fix postgres migration by @nguyer in https://github.com/hyperledger/firefly/pull/774

## New Contributors
* @keeganhrobinson made their first contribution in https://github.com/hyperledger/firefly/pull/649
* @calbritt made their first contribution in https://github.com/hyperledger/firefly/pull/755

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.14.1...v1.0.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-27 19:03:33 +0000 UTC
    </span>
</div>

