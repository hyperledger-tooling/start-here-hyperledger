---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1052" class=".btn">#1052</a>
            </td>
            <td>
                <b>
                    test-network-nano-bash chaincode id and waitForEvent improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use calculatepackageid to set CHAINCODE_ID
- Use waitForEvent to wait for commit event intead of 2s sleep
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 20:57:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1049" class=".btn">#1049</a>
            </td>
            <td>
                <b>
                    Update token_contract.go, modify the overflow judgment condition for function add().
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The general overflow  judgment condition for function add is not in every case.
for example, b = 5, q = -3, sum = 2, 
if (sum < q) == (b >= 0 && q >= 0) wil be true.
I modify this line for making it satisfied with every case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 06:32:50 +0000 UTC
    </div>
</div>

