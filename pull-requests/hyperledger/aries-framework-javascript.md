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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1462" class=".btn">#1462</a>
            </td>
            <td>
                <b>
                    fix: Registered Connection Problem report message handler
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
        Created At 2023-05-19 08:25:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1461" class=".btn">#1461</a>
            </td>
            <td>
                <b>
                    docs: update meeting link and time in  readme
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
        Created At 2023-05-19 07:57:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1459" class=".btn">#1459</a>
            </td>
            <td>
                <b>
                    test: tests for DidComm V2 message packing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added tests for DidComm V2 message packing
- Fixed issue to pass test vectors from the spec:  https://identity.foundation/didcomm-messaging/spec/#appendix

**Issue with the current implementation**: we need to use DID Resolver to unpack messages properly:
- resolve sender key from `skid`
- resolve recipient key from `kid`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 12:42:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1458" class=".btn">#1458</a>
            </td>
            <td>
                <b>
                    feat: DIDComm V2 messaging support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is follow up PR of: https://github.com/hyperledger/aries-framework-javascript/pull/1096
Chanegs:
* Merged with the main branch and solved conflicts
* Used combination of Askar and AFJ methods to support DIDComm V2 messaging instead of using Sicpa library
    * Implemented required crypto using Askar (Inds-SDK wallet do not support DIDComm V2)
    * Implemented required didcomm logic using existing AFJ (DidDocument resolving, Forward wrapping)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 14:38:32 +0000 UTC
    </div>
</div>

