---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Added support for fromBlock when generating eventservice cache keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The current cache key only takes into account the channel ID, which means if I have a different `fromBlock` number with a subsequent `RegisterBlockEvent()` call, it would not take effect because the previous event service will be returned from the cache lookup.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 22:40:42 +0000 UTC
    </div>
</div>

