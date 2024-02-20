---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    fix: empty stream state on broadcast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a broadcast is attempted and the steam state hasn't been initialise it caused a nil pointer.

Two ways to solve this:
- If the stream state is nil, set an empty one as part of broadcast but that means no connections will receive those messages until that map updates 
- Wait for a least one connection on this stream to start and then start broadcasting. At least one connection will receive the messages for the stream whilst it's connected

I've gone for the latter one. We perform best-effort delivery for broadcast, so it could be argued to do the former, any thoughts appreciated! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 12:12:15 +0000 UTC
    </div>
</div>

