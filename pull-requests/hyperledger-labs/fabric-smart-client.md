---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/320" class=".btn">#320</a>
            </td>
            <td>
                <b>
                    Use time.NewTimer instead of time.After
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using time.After enqueues an entry in Go's runtime scheduler and doesn't garbage collect it even if the function the timer was fired from terminates.
As a result, there can be a temporary high memory pressure and it degrades performance.

Replaced all places where time.After was used except in places that are used as samples or tests.

Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 15:46:23 +0000 UTC
    </div>
</div>

