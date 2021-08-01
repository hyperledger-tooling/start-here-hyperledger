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

