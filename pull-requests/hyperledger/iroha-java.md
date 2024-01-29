---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    Fixed RegistrableBox metadata merging for test genesis blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Before the map to determine the relation between metadata and instruction didn't care about the entity identifier so when there were multiple entities with the same metadata being registered all but one got removed from the resulting genesis.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 10:57:50 +0000 UTC
    </div>
</div>

