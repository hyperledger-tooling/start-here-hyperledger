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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    typescript_app: typescript build fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the typescript_app build error

@brioux 
 
Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 16:29:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    added status badges of GitHub Action pipelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
![image](https://user-images.githubusercontent.com/39259938/138733476-3db9f884-deab-4b82-9bcf-8d17e3cc5427.png)
![image](https://user-images.githubusercontent.com/39259938/138733411-0d426805-85f4-4f32-b69c-5646a6497641.png)

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 16:21:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/329" class=".btn">#329</a>
            </td>
            <td>
                <b>
                    Implement pre-commit hook for linting typescript_app and chaincode/typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements pre-commit hook using husky, which is being used for linting ``typescript_app`` and ``chaincode/typescript``.

Closes #324 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-23 15:28:23 +0000 UTC
    </div>
</div>

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

