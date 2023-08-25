---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1551" class=".btn">#1551</a>
            </td>
            <td>
                <b>
                    fix(transport): Use connection in WebSocket ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated `WsOutboundTransport` to use `connectionId` as part of WS connection identifier. In current implementation, only `endpoint` value is used.

This change fixes issue in use cases where tenant agent acts as a mediator:
- For instance, we have mediator and issuer agents hosted inside same multi-tenant AFJ instance and we also have a holder agent on mobile device. Holder on a mobile device has an active WS connection with a mediator.
- Currently, WS connection will be reused if it's already open for the same endpoint. This means that message sent from holder to issuer via WS transport will go through mediator WS connection
- On multi-tenant instance side, this message will be received with existing transport session of mediator WS connection
- This will cause transport session (along with mediator WS connection) to be closed as message addressed to issuer will not specify `return_route` (see [implementation](https://github.com/hyperledger/aries-framework-javascript/blob/main/packages/core/src/agent/MessageReceiver.ts#L148))
- Closed WS connection will trigger reconnection process

Above-metioned issue is causing unnecessary load in mediator interaction and may cause overlapping reconnection processes if there are a lot of messages being sent from holder to issuer in a short period of time (in our case, we were testing this with large amount of credential offers being accepted one by one).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 19:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1550" class=".btn">#1550</a>
            </td>
            <td>
                <b>
                    feat: did:peer:2 support in DID Exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some initial work on supporting `did:peer:2` in DID Exchange protocol, in order to start aligning with [RFC 0793](https://github.com/hyperledger/aries-rfcs/blob/fcb2cafce6abea0995804c32a6da473c8894e470/features/0793-unqualfied-dids-transition/README.md).

Currently, AFJ uses qualified DIDs for DID Exchange protocol, in `did:peer:1` format. The community is going towards `did:peer:2` and the new `did:peer:3` (more meaningful in DIDComm v2 world). So in this PR we are trying to do the transition from `did:peer:1` to `did:peer:2` in order to be compatible with ACA-Py when it adds support for the reception of qualified DIDs in DID Exchange protocol.

At the moment, the logic is the following:
- There is a new setting in `ConnectionsModuleConfig` to choose the default DID Peer num algo to use in DID Exchange Requests. If not defined, did:peer:1 will be used (this is current behaviour)
- There is a new optional setting in both OOB Reception and Invitation acceptance methods to override default setting. The use case would be: we know our mediator supports only `did:peer:2` (ACA-Py) so we connect with it using that algo, while still using `did:peer:1` for other agents (AFJ, AFGo)
- In DID Exchange Responses, we use the num algo the requester has used. So if they used `did:peer:2`, we'll respond with a `did:peer:2` as well, regardless of our default setting

Note: when using `did:peer:2`, both DID Exchange Requests and Responses are not adding any signature. There is an [open question](https://github.com/hyperledger/aries-rfcs/issues/717) since the time when DID Exchange was implemented in AFJ: I think we'll need to push to clarify this in order to have a common implementation in both AFJ and ACA-Py.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 15:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1549" class=".btn">#1549</a>
            </td>
            <td>
                <b>
                    fix: create message subscription first
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                mediation initialization was happening before the message subscription was registered, thus meaning the received messages to provision the mediator wouldn't be processed. This moves it to the start of the initialize method, before mediation initialization
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 12:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1548" class=".btn">#1548</a>
            </td>
            <td>
                <b>
                    chore(release): v0.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release version 0.4.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 11:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1547" class=".btn">#1547</a>
            </td>
            <td>
                <b>
                    fix(cheqd): make cosmos payer seed optional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Makes the cosmos payer seed optional, as you can also used it as a holder without payer seed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 10:45:53 +0000 UTC
    </div>
</div>

