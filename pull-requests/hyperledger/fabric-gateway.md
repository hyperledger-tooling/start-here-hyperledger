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
                `@noble/curves` makes use of `@noble/hashes`, which does not function correctly on big-endian systems, and also throws an error on module load if a big-endian system is detected. Revert to using elliptic as the ECDSA signing implementation.

Closes #628
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-09 14:40:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Remove dev dependency on jsrsasign
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor generation of key identifiers for hardware security module configuration in Node scenario tests to use Node crypto library, avoiding the need for dependency on jsrsasign.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-04 09:13:33 +0000 UTC
    </div>
</div>

