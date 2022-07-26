---
layout: default
title: business-partner-agent-chart
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent-chart
---

# business-partner-agent-chart <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent-chart){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    fix seed generation and ledger registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                see: https://github.com/hyperledger-labs/business-partner-agent-chart/issues/53

- removed automatic seed generation.
- had to keep a default value, because otherwise the tests will not run anymore. 
- set acapy admin key. 
- removed not needed acapy start params.
- removed idu ledger registration because it is not portable

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 09:55:21 +0000 UTC
    </div>
</div>

