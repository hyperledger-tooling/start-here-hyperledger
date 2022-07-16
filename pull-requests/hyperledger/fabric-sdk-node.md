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
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    Prevent race condition producing partial discovery results
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Discovery results parsing makes use of partial results, but these should not be set on the discovery service itself during the parsing process to ensure no callers ever see partial discovery results.

In combination with the above behaviour, the way the Contract obtained discovery results was prone to race conditions that could cause multiple discovery services to be created and invoked under load, and for partial discovery results to be obtained.

Closes #601
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 20:41:00 +0000 UTC
    </div>
</div>

