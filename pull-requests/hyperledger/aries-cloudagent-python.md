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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1302" class=".btn">#1302</a>
            </td>
            <td>
                <b>
                    Fix warnings due to action API updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 18:53:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1301" class=".btn">#1301</a>
            </td>
            <td>
                <b>
                    fix: failure to verify jsonld on non-conformant doc but vaild vmethod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor fix for jsonld verify route.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 18:22:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1300" class=".btn">#1300</a>
            </td>
            <td>
                <b>
                    Accept short DIDs for their_public_did parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow-up to https://github.com/hyperledger/aries-cloudagent-python/pull/1296
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 16:27:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1298" class=".btn">#1298</a>
            </td>
            <td>
                <b>
                    check if did is already qualified
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #1296 introduced a problem that  when the `pthid` got set to the public DID in a DIDX request with an already qualified DID it would still get prefixed with `did:sov`.


Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 17:35:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1297" class=".btn">#1297</a>
            </td>
            <td>
                <b>
                    Update version to 0.7.0-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 15:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1296" class=".btn">#1296</a>
            </td>
            <td>
                <b>
                    Support generic public DIDs in DIDX request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Be more permissive in validation of target public DID in `didexchange/create-request`.
Public DIDs are resolved using the resolver interface which supports additional DID methods besides `did:sov` (e.g. `did:web`).

Only question is if we should still allow unqualified DIDs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 12:56:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1294" class=".btn">#1294</a>
            </td>
            <td>
                <b>
                    DIF PE - is_holder property implementation - compliant with DIF spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1261
- I think this meets the following attributes from the DIF spec but does not use the `is_holder` property to decide whether the `VP` should be signed or not. But in case, this is needed then this can be done with minimal changes/extension.
1. `Verify that the Holder or Subject of the Claim still controls the identifier [DID].` [Link](https://identity.foundation/presentation-exchange/#proof-of-identifier-control)
2. `Holder of  Claim is the same as the Subject of the attribute.` [Link](https://identity.foundation/presentation-exchange/#note-2) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 11:21:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1293" class=".btn">#1293</a>
            </td>
            <td>
                <b>
                    Add indy-vdr test coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Basic unit test coverage
- Split out unit tests for `Role` class
- Move `taa_digest` implementation to base class
- Update indy-vdr version
- Implement `txn_endorse` for IndyVdrLedger

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 03:40:49 +0000 UTC
    </div>
</div>

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

