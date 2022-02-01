---
layout: default
title: orion-sdk-go
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-sdk-go
---

# orion-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-sdk-go/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Add SetClusterConfig method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add SetClusterConfig method in order to allow the full range of config changes.
- Also UpdateCAConfig method to allow easy updates to CA config.

Raft parameters are not exposed with their own method, but they can be updated using the
SetClusterConfig method.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 15:39:22 +0000 UTC
    </div>
</div>

