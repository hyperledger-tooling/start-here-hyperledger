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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/576" class=".btn">#576</a>
            </td>
            <td>
                <b>
                    Update "hyperledger-labs" references to "hyperledger", and fix linter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the "hyperledger-labs" references to "hyperledger".

Also, it fixes a problem with the linter. Namely, some golinter functions work with a top folder that is one level above the current one. Hence, when called from `FPC_PATH`, they start working from `FPC_PATH/..`. Others work from `./`. Finally, cpplinter works from one level above the scripts folders. This PR harmonizes these differences passing the top folder (i.e. `FPC_PATH`) as input to both scripts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 22:49:06 +0000 UTC
    </div>
</div>

