---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    Changing acme initialization to be like Alice and Faber ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ana Maria Franco Cuesta <afrancoc2000@gmail.com>
Fixing the issue [here](https://github.com/hyperledger/aries-cloudagent-python/issues/1288)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-04 17:19:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1287" class=".btn">#1287</a>
            </td>
            <td>
                <b>
                    Fix handling of empty accum_from in revocation state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also adds support for endorser_did/write_ledger params
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-03 01:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    Add outbound message transport events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces events relating to outbound messages. These changes are looking forward to more separation between the core ACA-Py message processing and generation components and message delivery mechanisms, which is fraught with nuance and largely dictated by use case. In such a state where there is a separation between message generation and delivery, we propose that these events (and/or similar events) act as the primary interface between the two. For now, however, these events are simply emitted and do not replace any of the previous functionality with one significant exception: considering how `OutboundSendStatus` was returned up the call stack from `outbound_message_router` and beyond, an `OutboundStatusEvent` seemed preferable. This change is mostly self-contained except for the recent `forward` message handler additions made to help with emitting push notifications to clients of mediators.

@TimoGlastra we were hoping to get your opinion on this change. As implemented, do you think the new `OutboundStatusEvent` would provide enough context to a push notifier or do we want to continue with a specific forward message event encapsulating the send status of the forwarded message?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 20:41:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1285" class=".btn">#1285</a>
            </td>
            <td>
                <b>
                    Format cred_rev_id as a string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes several AATH tests by formatting the `cred_rev_id` of a credential info structure as a string, not a number (Askar/Credx backend).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 03:28:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1284" class=".btn">#1284</a>
            </td>
            <td>
                <b>
                    PR#1276 Rework - Moved sorting of VCRecords into VCHolder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Following discussion with Andrew, decided to move the sorting logic into `./storage/vc_holder` for all 3 backends. 
- If there is a `dateutil` exception triggered when sorting then return the `records` list as it is
- Reverted changes made to `./present_proof/v2_0/formats/dif/handler.py`, `./present_proof/v2_0/routes.py` and corresponding tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 23:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1283" class=".btn">#1283</a>
            </td>
            <td>
                <b>
                    Remove indy-sdk dependency in IndyDidResolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `BaseLedger` interface ((it should really be called `IndyLedger`) is sufficient and allows indy-vdr to substitute.

This PR also changes the requirement checks in the demo agents to allow running without indy-sdk.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 20:20:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1282" class=".btn">#1282</a>
            </td>
            <td>
                <b>
                    Revert create schema and cred_def json response (remove 'sent')
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Makes the json response consistent with the previous aca-py release

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 14:15:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1281" class=".btn">#1281</a>
            </td>
            <td>
                <b>
                    OOB explicit invitations - Workaround for missing invitation_msg_id in webhook payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - To fix explicit invitations AATH tests
- Got approval from @nodlesh, ready to be merged 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 23:59:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1280" class=".btn">#1280</a>
            </td>
            <td>
                <b>
                    DIDExchange Error Fix - /didexchange/create-request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 20:26:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1276" class=".btn">#1276</a>
            </td>
            <td>
                <b>
                    DIF PE - giving Holder more control on how to specify presentation_request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1262 
[includes detail about the approach and discussion around the use cases]
- Maybe `./demo/AliceWantsAJsonCredential.md` needs to be updated
1. With no `auto` settings on. if multiple credentials are applicable to a `presentation_request` then it is required for `holder` to specify the credential `record_id`.

```
"record_ids": {
     "citizenship_input_1": [ "1496316f972e40cf9b46b35971182337" ]
}
```
2. With `auto` settings on, if X credentials are applicable to a `presentation_request` and only Y credentials should be returned based upon `submission_requirements`, then first Y credentials sorted by `issuanceDate` [in reverse] are returned.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 08:00:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1275" class=".btn">#1275</a>
            </td>
            <td>
                <b>
                    Update bdd tests to support askar; fix ledger method signatures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ledger methods are updated to provide endorser support for revocation updates

bdd updates are to allow tests to be run using askar wallet

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 21:18:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1274" class=".btn">#1274</a>
            </td>
            <td>
                <b>
                    Add `wait_for_event` method on event bus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've found this to be generally useful in some of our coding efforts and after a brief discussion with @esune noting that it would be of use in some of his ongoing work, we figured it would be good to pop this out of our ongoing work so it can be used elsewhere.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 20:01:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1272" class=".btn">#1272</a>
            </td>
            <td>
                <b>
                    Connection protocol used in ConnRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Now able to tell if a ConnRecord was created using `0160`, `0023` and `0023 with didcomm v2 envelope` [in future]
- Should fix AATH connection tests, as `connection_protocol` can be used instead of relying on `missing invitation_msg_id` which is no longer the case as to support connection_reuse [`RFC 0434`]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 18:00:13 +0000 UTC
    </div>
</div>

