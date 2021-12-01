---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v3.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v3.1.0
                </span>
            </td>
            <td>
                ## What's Changed
* ES Subscriptions: Store checkpoint after a stale subscription is processed by @vdamle in https://github.com/hyperledger/firefly-ethconnect/pull/157
* Add circuit breaker to stop runaway producers losing messages, and immediate receipt option by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/175
* Fix for intermittent failure #179 by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/180
* POST to /subscriptions with in-line event definition by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/177
* Add error codes to all ethconnect errors by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/178
* Make requestABIId omitempty by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/161
* Reduce default fetch below 1MB in the case of a small circuit breaker upper bound by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/181
* Fix post-merge build issue related to error codes by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/184
* Do not close a.eventStream, rather handle closed batch dispatcher by @peterbroadhurst in https://github.com/hyperledger/firefly-ethconnect/pull/183
* don't swallow webhook processMsg status codes by @shorsher in https://github.com/hyperledger/firefly-ethconnect/pull/187


**Full Changelog**: https://github.com/hyperledger/firefly-ethconnect/compare/v3.0.5...v3.1.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-01 15:31:41 +0000 UTC
    </span>
</div>

