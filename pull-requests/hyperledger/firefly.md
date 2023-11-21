---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1427" class=".btn">#1427</a>
            </td>
            <td>
                <b>
                    Fix JSON schema output for custom contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously we were generating an incorrect JSON Schema for the response body on custom contract endpoints. This PR fixes this so that:

- `/inovke` endpoints always return the correct schema for a FireFly Operation (which is the actual payload they return)
- `/query` endpoints now return the correct schema based on the return value of the smart contract itself
  - If outputs are unnamed, the swagger generator now names them `output`, `output1`, `output2`, etc. like ETH/EVMConnect name them
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 19:27:13 +0000 UTC
    </div>
</div>

