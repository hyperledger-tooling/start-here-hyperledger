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

Single Key-Value Storage (SKVS) is a naive approach for rollback attacks. All key-value pairs are encapsulated and stored in this approach with a single call to put_state(). During execution, the enclave must load the entire state before accessing individual key-value pairs. While this approach prevents the rollback attack, applications with large states and multiple writers will experience bad performance, as the use of a single key-value pair will cause transactions to fail due to concurrent write issues.

A user can use it by changing the chain code to SVKS chaincode
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

