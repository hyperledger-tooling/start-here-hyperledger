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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/542" class=".btn">#542</a>
            </td>
            <td>
                <b>
                    wip: add sql backend for token storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a service with datastores for tokens and the raw PublicParams. 

Work in progress:
- The current version only handles 1 database per instance, whereas it may be necessary to open different ttxdb based on the passed wallet id (to be discussed).
- Amount not stored as int yet (requires method signature change of Processor)
- Not plugged in to Vault, TokenStore or QueryExecutor yet. How to configure?
- TxStatus to be discussed.
- Some assorted small TODOs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-04 19:46:06 +0000 UTC
    </div>
</div>

