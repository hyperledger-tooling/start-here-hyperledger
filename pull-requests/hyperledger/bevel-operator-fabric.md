---
layout: default
title: bevel-operator-fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel-operator-fabric
---

# bevel-operator-fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel-operator-fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-operator-fabric/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    Add transient map arg to chaincode invoke&query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### What this PR does / why we need it:
In fabric peer chaincode (https://github.com/hyperledger/fabric/blob/main/internal/peer/chaincode), users can set transient map with argument `--transient`. 
In code -> https://github.com/hyperledger/fabric/blob/58b6dc3651e99db7e3eaa61285cac4c5b3cdef4d/internal/peer/chaincode/common.go#L579

There is no equivalent parameter in `kubectl hlf chaincode`. This pr solves that. 

#### Which issue(s) this PR fixes:
There is not any issue related with this problem.

#### Does this PR introduce a user-facing change?
Yes, users can set transient map in chaincode query&invoke comamnds.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 14:12:12 +0000 UTC
    </div>
</div>

