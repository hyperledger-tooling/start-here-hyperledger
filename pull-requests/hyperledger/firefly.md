---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1299" class=".btn">#1299</a>
            </td>
            <td>
                <b>
                    Fix unique indexes for transfers/approvals to be per-namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 16:54:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1298" class=".btn">#1298</a>
            </td>
            <td>
                <b>
                    fix-1297
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1297 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 19:03:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1296" class=".btn">#1296</a>
            </td>
            <td>
                <b>
                    Retry tokens events consistent with FFDX, as we cannot push back nack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make this consistent with what we did for FFDX, and prevents a scenario on startup as seen in the integration test where a token event comes in before the namespace is started:

```
firefly_core_0_1  | [2023-04-30T00:35:08.431Z] DEBUG Calling TokenPoolCreated callback. Locator='address=0x8875e026c26cedc2ab9880ac56d31e328428db73&schema=ERC20WithData&type=fungible' TX=token_pool/66fffabe-5b11-4118-abc2-50b95877654d pid=1 proto=fftokens role=event-loop
firefly_core_0_1  | [2023-04-30T00:35:08.431Z] ERROR Event loop exiting (FF10446: Namespace 'default' is not started). Terminating server! pid=1 proto=fftokens role=event-loop
```

Also made a change to both FFDX and FFTokens to split `eventRetry` out from `retry` in the config, as I realized looking at this PR that the config was overlapping with the `ffresty` config for request retry.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 04:24:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1295" class=".btn">#1295</a>
            </td>
            <td>
                <b>
                    Handle duplicate pool locators properly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since there is a unique index on pool locators, it must be checked during token pool upsert.

This behavior will be changing again in #1261, but this is a more immediate fix without pulling in all of that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 21:45:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1293" class=".btn">#1293</a>
            </td>
            <td>
                <b>
                    Remove duplicates prior to adding unique index on contract API ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also ensure ID is always unset when creating a new API.

Follow-up to #1292, #1275
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 19:46:08 +0000 UTC
    </div>
</div>

