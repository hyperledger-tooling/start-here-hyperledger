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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1454" class=".btn">#1454</a>
            </td>
            <td>
                <b>
                    fix: jsonld document loader node 18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the JSON-LD document loader in node 18. For now the node document loader is copied, but if https://github.com/digitalcredentials/jsonld.js/pull/2 is merged and released we can remove the custom implementation in AFJ.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 09:53:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1453" class=".btn">#1453</a>
            </td>
            <td>
                <b>
                    feat: support more key types in jws service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~~NOTE: this pr is dependant on #1446 and thus should be merged after that PR is merged.~~

This PR refactors the JWK and JWS implementation to have better support for JWK / JWA, and also support more algs/key types in the JWS service. Basically the JWS service now supports all JWKs supported in AFJ, although it's limited by the algs and key types supported by the wallet (for askar we support EdDsa and ES256)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 19:29:27 +0000 UTC
    </div>
</div>

