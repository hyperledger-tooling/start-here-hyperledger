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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    add tokengen function to update auditor and issuer certs in dlog pp files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the auditor or issuer certificate expires, we have to update it in the token chaincode. This action should *not* change the public parameters, because this would render existing tokens/proofs invalid.

This PR adds a command to the tokengen cli utility to update the auditor and/or issuers certificates in an existing `zkatdlog_pp.json`, without changing the public parameters.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 14:13:35 +0000 UTC
    </div>
</div>

