---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    F idemix aries
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
        Created At 2023-08-17 18:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/487" class=".btn">#487</a>
            </td>
            <td>
                <b>
                    idemix: validate identities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This PR addresses the following issue: For the DLog driver, the identity of a token owner was not validated against the Issuer public key. This PR makes sure that this happens and that validation enforces the presence of the commitments to the EID and RH respectively. 

1. add to the public params the revocation public key
2. when deserializing idemix identities, check the validity of the identity and forse the presence of the nyms
3. unit-test added
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 08:42:13 +0000 UTC
    </div>
</div>

