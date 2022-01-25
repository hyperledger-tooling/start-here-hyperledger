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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/311" class=".btn">#311</a>
            </td>
            <td>
                <b>
                    Fix Doc: Type of args in invokeChaincode() is string[]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                stub.invokeChaincode() receives a parameter `args` which is
a string array having arguments to pass to the called chaicode.
However, the current document explains the `args` is byte[][].
This PR fixes the document issue above.

Signed-off-by: Yuki Kondo <yuki.kondo.ob@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 01:18:15 +0000 UTC
    </div>
</div>

