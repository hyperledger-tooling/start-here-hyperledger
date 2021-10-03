---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/633" class=".btn">#633</a>
            </td>
            <td>
                <b>
                    Upgrade go and fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **What this PR does / why we need it**:

This PR upgrade go version to 1.16.7, the same version as currently used by Fabric. Also, we upgrade to the most recent version of Fabric 2.3.3. The main reason for upgrading to this fabric version is to resolve compatibility issues between 2.3.0 and 2.3.3 as already mentioned in #629. 

**Special notes for your reviewer**:
Note that in the test-network tutorial, we are now using the main branch for fabric-samples as there is no 2.3.3 tag yet available. The previous tag 2.3.0, we used, is not compatible with Fabric 2.3.3. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 11:13:05 +0000 UTC
    </div>
</div>

