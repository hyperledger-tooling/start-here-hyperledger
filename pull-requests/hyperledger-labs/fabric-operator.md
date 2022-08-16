---
layout: default
title: fabric-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operator
---

# fabric-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Use hyperledger-labs operator, not ibm-blockchain operator in sample network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After installing the operator about 50 times in test clusters, I was wondering why the image download counts from ghcr.io were still zero.  This would explain the issue... 

Sample network now pulls the LABS operator image, not the legacy rev (pre-labs).

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 01:20:36 +0000 UTC
    </div>
</div>

