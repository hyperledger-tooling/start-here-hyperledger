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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/198" class=".btn">#198</a>
            </td>
            <td>
                <b>
                    First argument should be of type Context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A transaction function must have at least one argument, which is of type Context.

Originally, if a transaction function has 0 arguments, the runtime exists. Now with this PR, the runtime gives some cues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 05:55:37 +0000 UTC
    </div>
</div>

