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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    ZKATDLOG: Improved VaultTokenCommitmentLoader
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                The current loader fails if the commitment of a given token does not exists, but it might be that the corresponding transaction is still pending. This means that the commit pipeline hasn't had time to process the transaction yet.

This PR improves the loader by adding the possibility to retry after some time. 

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 15:55:30 +0000 UTC
    </div>
</div>

