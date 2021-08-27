---
layout: default
title: blockchain-verifier
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-verifier
---

# blockchain-verifier <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-verifier){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-verifier/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Skip processing key-value pairs unless necessary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the current implementation, key-value processing can take much time and memory to save the history of all the values in the state. This patch skips key-value pairs when no application checkers are specified.

This suppresses time and memory consumption when a user does not intend to examine and verify the contents of the transactions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 07:02:57 +0000 UTC
    </div>
</div>

