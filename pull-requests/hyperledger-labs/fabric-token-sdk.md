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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    ttxdb derivates: failed restart #402
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This PR fixes the `owner` and `auditor` services. Before, these services were not able to recover from a shutdown of the node. Now, at bootstrap, the services first check if there are transactions whose status is still pending and for those a commit listener is added. 

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-09 10:59:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    Update Public Param
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 14:39:00 +0000 UTC
    </div>
</div>

