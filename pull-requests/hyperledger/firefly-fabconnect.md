---
layout: default
title: firefly-fabconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Update fabconnect to send receipts conforming to FireFly receipt stru…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …cture

See PR https://github.com/hyperledger/firefly/pull/1111 which standardises the format of a blockchain receipt notification to FireFly core. The standard structure defined in that PR requires transaction hash to be represented as a common field between all blockchain connectors. Before now Fabconnect used `transactionId` and ethconnect used `transactionHash`, and hence each plugin in FireFly core had its own logic for parsing transaction receipts. PR https://github.com/hyperledger/firefly/pull/1111 standardises on `transactionHash` so this PR brings fabconnect into line with that change. This allows FireFly core to have common blockchain receipt processing code.

Signed-off-by: Matthew Whitehead <matthew.whitehead@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 11:31:46 +0000 UTC
    </div>
</div>

