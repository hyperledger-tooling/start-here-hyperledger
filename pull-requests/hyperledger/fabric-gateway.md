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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    Use SHA256 to hash salted creator bytes for transaction ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Code previously used whichever hash function the client supplied when connecting the Gateway. For some implementations this hash function may use a different algorithm or even just pass through bytes unchanged. Fabric requires that the salted creator bytes be SHA256 hashed when generating a transaction ID. Any other algorithm would cause an invalid transaction ID to be generated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 12:20:13 +0000 UTC
    </div>
</div>

