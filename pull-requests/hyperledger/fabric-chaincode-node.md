---
layout: default
title: fabric-chaincode-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-node
---

# fabric-chaincode-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/349" class=".btn">#349</a>
            </td>
            <td>
                <b>
                    Add fv test chaincode deploy logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously if chaincode deploy failed during fvt tests no message was logged making it impossible to troubleshoot. Now the chaincode deploy commands and results and logged.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 17:13:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/348" class=".btn">#348</a>
            </td>
            <td>
                <b>
                    Update release-2.2 to use Fabric v2.4.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix test failure related to the use of 2.3.x peer binary. peer binary  2.3.x did not have calculatepackageid implemented, which fabric-samples now uses. Ideally tests should not depend on fabric-samples.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 18:37:07 +0000 UTC
    </div>
</div>

