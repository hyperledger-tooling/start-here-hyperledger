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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1451" class=".btn">#1451</a>
            </td>
            <td>
                <b>
                    feat(indy-vdr): schema + creddef endorsement
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
        Created At 2023-05-10 12:03:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1450" class=".btn">#1450</a>
            </td>
            <td>
                <b>
                    fix: remove scope check from response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the `requestCredential` method would throw an error if the `scope` parameter was not present in the `access_token` response. This `scope` value was used to indicate the desired credential type when requesting the credential. However, this was incorrect, as this value is optional according to the [specification](https://www.rfc-editor.org/rfc/rfc6749.html#section-4.2.2).

This PR removes the requirement for the `scope` to be present on the `access_token` response. If the `scope` is present, it will be used to check if the server metadata indicates the requested credential format is supported for the requested credential type (indicated by the `scope`). If not, this validation is skipped.

When the `access_token` response does not contain a `scope`, the `credentialType` value that is passed to the underlying Sphereon library will be undefined. When this happens, the Sphereon library will use the `credentialType` value from the issuance initiation request instead (relevant code [here](https://github.com/Sphereon-Opensource/OID4VCI/blob/56b16a33fe8826043906f1d82616f0a9a0873d75/lib/CredentialRequestClient.ts#L66)), which should always be present according to the [spec](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0-09.html#section-e.1.1.3).

@TimoGlastra, @blu3beri, could one of you please verify these changes are in line with the specs? 

Related to #1322 

Signed-off-by: Karim Stekelenburg <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 17:51:18 +0000 UTC
    </div>
</div>

