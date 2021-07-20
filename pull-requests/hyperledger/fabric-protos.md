---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    [FAB-18527] Hint to discovery to disregard the namespace endorsement policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    
This commit adds a hint in the chaincode call of the discovery protobuf API
to signal that the client expects the namespace endorsement policy to be irrelevant.


Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 12:25:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    FABGW-25 Extend proto to include derived interest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add protobuf support for returning the derived chaincode interest structure from Tx simulation (process proposal).

Add the set of SBE signature policies to the discovery ChaincodeCall proto message
Add the ChaincodeInterest structure to the ProposalResponse message

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 15:50:51 +0000 UTC
    </div>
</div>

