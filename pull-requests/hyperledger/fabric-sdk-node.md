---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/538" class=".btn">#538</a>
            </td>
            <td>
                <b>
                    Fix regression in ECDSA_KEY.generateCSR() (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of PR #537 to release-2.2 branch.

Subject alternative names extensions were not being correctly handled. Moving to non-deprecated jsrsasign API call and implementing some translation between previous extension format and the one required by the new API call.

Contributes to #536 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-05 21:08:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/537" class=".btn">#537</a>
            </td>
            <td>
                <b>
                    Fix regression in ECDSA_KEY.generateCSR()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Subject alternative names extensions were not being correctly handled. Moving to non-deprecated jsrsasign API call and implementing some translation between previous extension format and the one required by the new API call.

Resolves #536
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 22:41:35 +0000 UTC
    </div>
</div>

