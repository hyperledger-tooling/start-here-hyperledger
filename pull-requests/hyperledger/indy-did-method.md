---
layout: default
title: indy-did-method
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-did-method
---

# indy-did-method <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-did-method){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    docs: remove DIDDoc validation requiring current DID Core JSON-LD context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is the product of the discussion in Issue #57. This DID Core context validation does not ensure that the resulting JSON-LD DIDDoc is valid and it would need to be updated if the DID Core context is changed. It is the responsibility of the content creator to validate that the resulting DIDDoc is valid JSON-LD. 

Signed-off-by: Char Howland <char@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 05:57:42 +0000 UTC
    </div>
</div>

