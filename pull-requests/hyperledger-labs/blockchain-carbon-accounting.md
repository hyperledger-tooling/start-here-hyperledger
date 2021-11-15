---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    feat (test): Test if partyId is being hashed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The SHA-256 hash of the `partyId` is computed before it is stored as an emission record so as to maintain confidentiality. This PR adds a test that exercises this functionality by computing the hash of the `partyId` separately and then asserting that the hash stored on the ledger matches the separately computed hash.

Closes #187. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 07:53:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    REST API for ws-wallet web-socket-key request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ws-wallet REST API to request and authorize web-socket keys for third party applications

POST /session/new/ ,
body: {endpoint: <fabric app's ws-identity session ticket  url>, key_name: <keyName>}

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 03:56:05 +0000 UTC
    </div>
</div>

