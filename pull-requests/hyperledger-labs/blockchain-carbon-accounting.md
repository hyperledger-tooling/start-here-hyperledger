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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    Add identity router for differnet signer types
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    small changes to docs with link to secure identities directories
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Si Chen <sichen@opensourcetrategies.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 22:28:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Lint warning fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hacktoberfest-accepted</span>
            </td>
            <td>
                Fixes #305 

* Fixed lint warning in chaincode

* Fixed linting warnings in typescript_app

* Fixed lint warning due to prettier auto save
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 19:38:54 +0000 UTC
    </div>
</div>

