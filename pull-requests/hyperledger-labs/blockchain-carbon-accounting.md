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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/326" class=".btn">#326</a>
            </td>
            <td>
                <b>
                    Vault identity Management server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add Vault identity Management server for managing vault identity for the client. 

Close #312 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 18:49:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    Add identity router for different Fabric types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes a dedicated identity router for setting up API keys for different signer types

Revised procedure for issuing web-socket session keys:
1. Mobile app requests userId and generates a key file using ws-wallet
2. pub key is passed to express API path _/identity/webSocket_ to request session ID ticket
3. The mobile app/wallet receives _sessionId_ and _url_ response to open ws connection with ws-identity
4. Sends SessionId/Signature API pair to open connection and authenticate express API txs

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 11:41:19 +0000 UTC
    </div>
</div>

