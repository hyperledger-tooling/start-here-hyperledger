---
layout: default
title: hlf-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hlf-operator
---

# hlf-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-operator/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Fix kubectl-hlf inspect command when empty peer array
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found this bug while playing around with the operator, if organization has no peers it results in an error:

`network configuration load failed: failed to parse 'peers' config item to endpointConfigurationEntity.Peers type: '' expected a map, got 'slice'`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 10:18:48 +0000 UTC
    </div>
</div>

