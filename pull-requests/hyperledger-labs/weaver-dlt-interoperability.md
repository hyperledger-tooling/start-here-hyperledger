---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/379" class=".btn">#379</a>
            </td>
            <td>
                <b>
                    Bug Fix in Interop Node SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **BUG**: There's a bug in `GetSubscriptionState` in Weaver Fabric SDK, which doesn't work when `ContractTransaction` is not present in `EventPublicationSpec`, i.e. when `appURL` is used for subscription, as there's few lines of code which only works with `ContractTransaction` in event publication spec.

**FIX**: Added a safety check `EventPublicationSpec.hasCtx()` around the code to fix it, which checks if the `EventSubscription` has `ContractTransaction` then only it executes the code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 10:17:16 +0000 UTC
    </div>
</div>

