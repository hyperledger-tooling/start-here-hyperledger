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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Update versions following v1.3.2 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 17:37:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    Use elliptic instead of @noble/curves for Node crypto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `@noble/curves` makes use of `@noble/hashes`, which does not function correctly on big-endian systems, and also throws an error on module load if a big-endian system is detected. Revert to using `elliptic` as the ECDSA signing implementation.

Closes #628
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-09 14:40:51 +0000 UTC
    </div>
</div>

