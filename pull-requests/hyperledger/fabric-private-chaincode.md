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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    Feature/solution skvs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **What this PR does / why we need it**:

Implement a Rollback attack protection solution for FPC: SKVS.
user can choose to use it by changing the chaincode to SVKS chaincode
ex: `skvsChaincode := fpc.NewSkvsChaincode(secretChaincode)`


**Which issue(s) this PR fixes**:
Fixes #484 

**Special notes for your reviewer**:
Loom demonstration video: [Watch here](https://www.loom.com/share/4790cd0cba9e4433879083b41158d42d?sid=a0f367e7-dc49-4065-926d-df7b2fbf55a1)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 12:56:04 +0000 UTC
    </div>
</div>

