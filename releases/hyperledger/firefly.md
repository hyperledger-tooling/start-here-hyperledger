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
                    v0.13.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.13.1
                </span>
            </td>
            <td>
                ## Summary
* Support for [token approvals](https://github.com/hyperledger/firefly/pull/529) (only supported by erc1155 connector as of this release)
* Bug fixes

## Updated Dependencies

* firefly-ethconnect [v3.1.4](https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.4)
* firefly-fabconnect [v0.9.11](https://github.com/hyperledger/firefly-fabconnect/releases/tag/v0.9.11)
* firefly-tokens-erc1155 [v0.10.5](https://github.com/hyperledger/firefly-tokens-erc1155/releases/tag/v0.10.5)
* firefly-tokens-erc20-erc721 [v0.1.6](https://github.com/hyperledger/firefly-tokens-erc20-erc721/releases/tag/v0.1.6)

## What's Changed
* Add additional backwards compatibility check on ethereum instance path by @nguyer in https://github.com/hyperledger/firefly/pull/531
* Build a predictable response body for async "InvokeContract" calls by @awrichar in https://github.com/hyperledger/firefly/pull/532
* Add endpoint to automatically generate an FFI by @nguyer in https://github.com/hyperledger/firefly/pull/511
* Updates to DX by @gabriel-indik in https://github.com/hyperledger/firefly/pull/534
* Add Transaction ID to Events by @awrichar in https://github.com/hyperledger/firefly/pull/522
* Add query support for Fabric by @nguyer in https://github.com/hyperledger/firefly/pull/533
* [transfer-type-query] allow filtering by type on token transfers by @eberger727 in https://github.com/hyperledger/firefly/pull/544
* Change query method to POST for custom contracts by @nguyer in https://github.com/hyperledger/firefly/pull/542
* Fix empty swagger URLs on contract API creation by @nguyer in https://github.com/hyperledger/firefly/pull/543
* Support for token approvals by @shorsher in https://github.com/hyperledger/firefly/pull/529
* Docs "bundle update" to pick up new nokogiri build by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/552
* Documentation updates from @TheSwarnim by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/553
* Updated documentation to make it more useful by @TheSwarnim in https://github.com/hyperledger/firefly/pull/451
* Roll requestConflictEmptyResult from Group to Data and Message too by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/551
* Explicitly name all subscriptions by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/555
* Update manifest versions by @awrichar in https://github.com/hyperledger/firefly/pull/556

## New Contributors
* @gabriel-indik made their first contribution in https://github.com/hyperledger/firefly/pull/534
* @TheSwarnim made their first contribution in https://github.com/hyperledger/firefly/pull/451

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v0.13.0...v0.13.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v0.13.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-01 21:30:25 +0000 UTC
    </span>
</div>

