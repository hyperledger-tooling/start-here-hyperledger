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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1560" class=".btn">#1560</a>
            </td>
            <td>
                <b>
                    feat: credential protocols v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implementation of [Issue Credential V3](https://github.com/decentralized-identity/waci-didcomm/tree/main/issue_credential) and [Present Proof V3](https://github.com/decentralized-identity/waci-didcomm/blob/main/present_proof/present-proof-v3.md), based on V2 protocols and updating them to use attachments for DIDComm V2.

This is dependent on https://github.com/hyperledger/aries-framework-javascript/pull/1546 (as there are a few general corrections and tweaks for DIDComm V2 there) and there is still some work to do, such as:
- Add tests
- Add OOB support (if needed)
- Verify its correct alignment with WACI-DIDComm definitions in terms of message definitions and flow

At the current status, it allows to run all possible use-cases for AFJ demo (connect, send message, offer credential, request proof) in both DIDComm V1 and DIDComm V2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 17:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1559" class=".btn">#1559</a>
            </td>
            <td>
                <b>
                    fix: do not send package via outdated session
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We found an edge-case where a websocket transport session would be closed/unavailable on the client agent side, but mediator still thinks it is available (due to client being offline).
When client returns back online and initiates a flow via mediator, the mediator will attempt to send the package to the now outdated websocket, instead of the newest / current session.

This PR fixes the problem, but is there any reason why a single connection may need multiple open WebSocket transport sessions?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 14:15:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1558" class=".btn">#1558</a>
            </td>
            <td>
                <b>
                    fix(oob): support oob with connection and messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1129

We now correctly check whether an oob exchange is associated with an exchange if there's no connectionId, and assign the connection if this is the case. 

I think we now really support al flows and combinations of messages / handhsake / connectionless from the oob protocol.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 14:02:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1557" class=".btn">#1557</a>
            </td>
            <td>
                <b>
                    fix: bump missing dependencies version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a blocker in the docker file where the source openssl libs are no longer available.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 16:22:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1555" class=".btn">#1555</a>
            </td>
            <td>
                <b>
                    fix: priority sorting for didcomm services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1553 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 12:40:53 +0000 UTC
    </div>
</div>

