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
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/674" class=".btn">#674</a>
            </td>
            <td>
                <b>
                    Socket connection fix: destroy() used instead of abort()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While testing the `fabric-node-SDK`, found that the connections were not getting reused creating more connections in the pool. 

While debugging the issue further found that the issue is the connection was not getting destroyed. The `request.abort()` method was deprecated for a really long time too, so it makes sense this could be changed. 

Thus, this minor code change fixes this issue and we're able to decrease the number of active GRPC connections on the network.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 10:55:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    Reduce scheduled build frequency to weekly
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
        Created At 2023-05-09 14:26:16 +0000 UTC
    </div>
</div>

