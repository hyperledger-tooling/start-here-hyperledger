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
                    v1.0.0-rc.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-rc.6
                </span>
            </td>
            <td>
                ## What's Changed
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

## New Contributors
* @calbritt made their first contribution in https://github.com/hyperledger/firefly/pull/755

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.0-rc.5...v1.0.0-rc.6
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-26 22:04:48 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.0.0-rc.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-rc.5
                </span>
            </td>
            <td>
                ## What's Changed
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


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.0-rc.4...v1.0.0-rc.5
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.0-rc.5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-20 13:06:52 +0000 UTC
    </span>
</div>

