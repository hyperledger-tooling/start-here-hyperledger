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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1542" class=".btn">#1542</a>
            </td>
            <td>
                <b>
                    fix: listen to incoming messages on agent initialize not constructor
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
        Created At 2023-08-08 10:07:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1541" class=".btn">#1541</a>
            </td>
            <td>
                <b>
                    chore: DidCommV2: Sync with the main branch
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
        Created At 2023-08-06 09:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1540" class=".btn">#1540</a>
            </td>
            <td>
                <b>
                    fix: DidCommV2 - avoid breaking changes 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to avoid breaking changes compared to the main branches.

- Preserved export of `AgentMessage` class which actually is `DidCommV1Message`. 
  - `AgentBaseMessage` is a common interface for V1/V2 - used internally
- Preserved name `Attachment` for DidCommV1 message attachments       
- Preserved name `SigningProvider`

Differences with the `main`
- `outOfBandInvitation` field of the OutOfBand record is optional
  - Reason: for DidCommV2 added separate field `v2OutOfBandInvitation`   
- `TransportSession` - `keys` and `inboundMessage`refers to different types but it should not break implementations.



TransportSession
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 07:49:49 +0000 UTC
    </div>
</div>

