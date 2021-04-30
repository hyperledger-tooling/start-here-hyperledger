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
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/450" class=".btn">#450</a>
            </td>
            <td>
                <b>
                    [FABN-1710] Fix HSM persistance issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - wallet.md - save SKI instead of key handle in wallet (handle not valid between sessions)
- FabricCAServices.js - pass {persist: true} param to generateEphemeralKey in order for private key to be persisted in HSM
- hsmx509identity.ts - get private key using SKI from HSM in getUserContext()
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 14:10:47 +0000 UTC
    </div>
</div>

