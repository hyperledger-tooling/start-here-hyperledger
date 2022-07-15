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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    Swap to using the published fabric-protos libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move the codebase to directly using the published protobuf libraries. The fabric-protos
repo, as well as holding the 'main' copy of the protos, also publishes packages for each language
These can then be pulled directly here; everything under version control.

Removes the need to the copies of the protobufs held locally in this repo.

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 09:57:57 +0000 UTC
    </div>
</div>

