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
                Previously the `requestCredential` method would throw an error if the `scope` parameter was not present in the `access_token` response. This `scope` value was used to indicate the desired credential type when requesting the credential. However, this was incorrect, as this value is optional according to the specification.

Because we still need to provide a credential type when requesting the credential, I have added an optional `scope` parameter to the `RequestCredentialOptions` interface. If the `access_token` response includes the `scope`, that value will be used. If the `scope` value is not present on the `access_token` response, the `scope` parameter from the `RequestCredentialOptions` interface will be used. If both are not present, an error will be thrown.

Related to #1322 

Signed-off-by: Karim Stekelenburg <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 17:51:18 +0000 UTC
    </div>
</div>

