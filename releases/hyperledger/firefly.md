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
                    v1.0.0-rc.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-rc.2
                </span>
            </td>
            <td>
                ## What's Changed
* Configuration docs, and packaging config/i18n for re-use by microservices by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/678
* Fix make docker command in release build GitHub Action by @nguyer in https://github.com/hyperledger/firefly/pull/682
* Enforce config descriptions by @nguyer in https://github.com/hyperledger/firefly/pull/681
* Remove extra postgres migrations by @nguyer in https://github.com/hyperledger/firefly/pull/683


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.0-rc.1...v1.0.0-rc.2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-09 13:39:30 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-rc.1
                </span>
            </td>
            <td>
                ## Summary
* Significant performance improvements
  * More types of background workers
  * Better caching and indexing
  * Batching of database updates
* Greatly improved OpenAPI spec, including more accurate input/output params and text descriptions of all fields
* UI updates and general bug fixes

## Breaking Changes and Migrations
* **firefly-dataexchange-https** must be upgraded to the version listed below, as the ack event [has been renamed](https://github.com/hyperledger/firefly/pull/656) from "commit" to "ack". Running mismatched versions of FireFly and dataexchange in this case will cause event processing to stall completely.

## Updated Dependencies
* firefly-ethconnect [v3.1.6](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.6)
* firefly-dataexchange-https [v0.11.1](https://github.com/hyperledger/firefly-dataexchange-https/releases/tag/v0.11.1)
* firefly-tokens-erc1155 [v0.10.8](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v0.10.8)
* firefly-tokens-erc20-erc721 [v0.2.3](https://github.com/hyperledger/firefly-tokens-erc20-erc721/releases/tag/v0.2.3)
* firefly-ui [v0.6.10](https://github.com/hyperledger/firefly-ui/releases/tag/v0.6.10)

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

## New Contributors
* @keeganhrobinson made their first contribution in https://github.com/hyperledger/firefly/pull/649

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.14.1...v1.0.0-rc.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-08 19:31:24 +0000 UTC
    </span>
</div>

