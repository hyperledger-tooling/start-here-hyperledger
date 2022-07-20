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
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    Revert to snapshot publishing following release
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
        Created At 2022-07-19 12:42:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/609" class=".btn">#609</a>
            </td>
            <td>
                <b>
                    Release v2.2.14
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
        Created At 2022-07-19 11:43:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    Refactor DiscoveryService usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of b3799f6a0002a1478284737a95a3c073d67ee56c from main branch.

Discovery results parsing makes use of partial results, but these should not be set on the discovery service itself during the parsing process to ensure no callers ever see partial discovery results.

In combination with the above behaviour, the way the Contract obtained discovery results was prone to race conditions that could cause multiple discovery services to be created and invoked under load, and for partial discovery results to be obtained.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 10:10:35 +0000 UTC
    </div>
</div>

