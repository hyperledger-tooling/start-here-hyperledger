---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    Fix Context naming issues with inference contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Reuse vetting, asset, and issuer context from exchange modules for the inference jupyter module, rather than redefining. 
2. Renamed the inference specific contexts to prevent overwriting of exchange related contexts
3. With these changes, a single instance of jupyter container can be used to interact with both inference and exchange contracts
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 20:44:56 +0000 UTC
    </div>
</div>

