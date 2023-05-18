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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1456" class=".btn">#1456</a>
            </td>
            <td>
                <b>
                    fix!: return didcomm mime-type in http response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
BREAKING CHANGE:
previously the HttpInboundTransport would return a response content type of `application/json`. This is incorrect and lead to interoperability issues (especially with the Lissi wallet). As there's multiple mime-types that can be used the TransportSession.send method now takes an agentContext parameter to extract this from the config.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 12:59:56 +0000 UTC
    </div>
</div>

