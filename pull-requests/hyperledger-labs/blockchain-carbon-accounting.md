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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    bring open offsets project up to date
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
        Created At 2021-08-05 22:30:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    Move content of multiple .gitignore file to a single file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #269
Signed-off-by: Bhaarat Kumar Khatri <bharatkhatri351@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 09:47:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    Encrypt partyId with AES and remove SHA-256 hash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes #263  
- [x] Encrypt the partyId with AES cipher algorithm in the typescript_app when invoking the chaincode function recordEmission. The secret passphrase needs to be stored in the middleware.
- [x] Remove all functions that calculate the hash value of the partyId from the chaincode

Initially for this PR, as @udosson suggested, I am using a constant passphrase.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-01 09:26:41 +0000 UTC
    </div>
</div>

