---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    chore(docs): fix nodejs async for loop examples 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The block event examples do not seem to work and I have never heard of `for async`. I assume they are supposed to be `for await`, which is what the fabric samples use [here](https://github.com/hyperledger/fabric-samples/blob/c0a0104ca1ca9107cb7cea8af3758d1ec256df02/asset-transfer-events/application-gateway-typescript/src/app.ts#L79).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-14 14:36:07 +0000 UTC
    </div>
</div>

