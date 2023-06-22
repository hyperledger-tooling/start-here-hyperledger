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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1060" class=".btn">#1060</a>
            </td>
            <td>
                <b>
                    Fix transferFrom function in erc-1155 sample so that we only delete token balances after…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … we've verified the funds are available first - not before

Deleting the state before the necessary funds are identified first results in funds disappearing without a recipient receiving them since the transaction then results in an error state being returned.  

This update defers the deleteState calls so that they do not occur if `partialBalance < neededAmount` is true (not enough funds available)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 23:40:51 +0000 UTC
    </div>
</div>

