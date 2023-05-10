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

