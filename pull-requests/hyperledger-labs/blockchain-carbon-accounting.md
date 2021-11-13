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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/356" class=".btn">#356</a>
            </td>
            <td>
                <b>
                    feat(CI): Add tests for net-emissions-token-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added tests for `net-emissions-token-network` to the CI pipeline. @udosson as for uploading the test results, `npx hardhat test` does not provide any options as of now to export the test results, even though they are internally using Mocha. So, for the moment, it won't be possible to upload the test reports as an artifact to get the test reports using the `test-reporter` action. We could request the feature to export test reports [on their repo](https://github.com/nomiclabs/hardhat), or I could work on this if needed in the future.

Closes #292.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 11:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/355" class=".btn">#355</a>
            </td>
            <td>
                <b>
                    docs(CI): Add comments for CI pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added in-line comments to the YAML workflow files for the CI pipeline. Closes #307.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 07:13:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/354" class=".btn">#354</a>
            </td>
            <td>
                <b>
                    Add password encryption to PKCS#8 private key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    - ws-wallet new-key requests user to input password to encrypt PKCS#8 private key
    - ws-wallet open will request password to decrypt private key for signing
    - getPass() fn handles terminal requests to input passwor 
    - unlockKey() fn checks if decryption password is valid. Process closed after 3 failed attempts
    - Password -p option can be provided with new-key and open commands

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-06 21:05:58 +0000 UTC
    </div>
</div>

