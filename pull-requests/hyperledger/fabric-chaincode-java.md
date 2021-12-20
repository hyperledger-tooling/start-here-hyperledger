---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    Revert "add cause message to ContractRuntimeException message"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 16f6a6fe65cef59be8e9481e0e42574901f96cbb.

The ContractRuntimeException intentionally doesn't report any details back to the client for security reasons.

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 16:26:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    FCJ-214 improved ChaincodeRuntimeException message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #214 
improved ChaincodeRuntimeException message by adding payload to message response. So, users can see better described and more informative exception messages.
Signed-off-by: Oleksandr Yamkovyi <oleksandr.yamkoviy@intellecteu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 14:49:34 +0000 UTC
    </div>
</div>

