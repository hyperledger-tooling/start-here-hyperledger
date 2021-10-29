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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/336" class=".btn">#336</a>
            </td>
            <td>
                <b>
                    update documentation for ws-socket and vault security
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @brioux @Zzocker Can you please review these changes to the documentation based on our call on Monday?

I'm still not too clear where the ws-identity and ws-identity-client are vs each other. Does ws-wallet talk to ws-identity, which then talks through ws-identity-client to Fabric?

A client application that uses web socket identity then somehow incorporate ws-wallet in its UI?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 00:15:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    Updated tests for FabricSigningCredentialType.WsX509
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replicate existing tests for VaultX509
Add gateway interface IWebSocketKey for webSocketKey object with sessionId and signature.
Extend service/input header to include Record with object values (not just strings).

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 05:31:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    small changes to documentation
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
        Created At 2021-10-25 23:07:03 +0000 UTC
    </div>
</div>

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

