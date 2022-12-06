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
                PR <a href="https://github.com/hyperledger/iroha-java/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    Make validation for max description length configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The max length of the `description` property of TransferAsset message can be configured via genesis block.

https://iroha.readthedocs.io/en/main/develop/api/commands.html#id87

iroha-java client uses fixed max length to check the transaction. This commit remove the restriction and let the user configure the max length according to their needs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 10:26:20 +0000 UTC
    </div>
</div>

