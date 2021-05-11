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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/445" class=".btn">#445</a>
            </td>
            <td>
                <b>
                    Correct Javascript Chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - In CreateAsset, await was never called on putState causing issues
especially with tools such as caliper and is not correct practice.
Unfortunately all the other examples use `return` which works but is
actually not the idiomatic way of handling promises, so here await is
chosen rather than return
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 08:50:35 +0000 UTC
    </div>
</div>

