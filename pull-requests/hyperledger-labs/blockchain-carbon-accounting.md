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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Add test reports to CI pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds test reports to the existing CI test pipeline, using the [Test Reporter Action](https://github.com/marketplace/actions/test-reporter). For the purposes of creating the report, a new script called `test:ci` has been added in wherein Mocha has been configured to output to a `test-results.json` file (this functionality was added in with Mocha [v9.1.0](https://github.com/mochajs/mocha/releases/tag/v9.1.0)). This file is then uploaded using the [Upload Artifact Action](https://github.com/actions/upload-artifact). The test reporter workflow has been separated out into a new file [as specified here](https://github.com/marketplace/actions/test-reporter#recommended-setup-for-public-repositories).

Closes #291.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-23 07:46:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    Fix fabric-registry tests for web-socket signer type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 12:35:01 +0000 UTC
    </div>
</div>

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

