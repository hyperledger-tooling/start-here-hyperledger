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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    Support for websockets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Websocket client, small fixes for server and unit test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 16:12:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    bidirectional channel between the invoker of a view and the view itself
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This PR introduces the support for a bidirectional channel between the invoker of a view and the view itself.
This PR supports this channel in two ways:
- Using GRPC stream, and
- Using WebSockets

The `pingpong` integration test has been extended to test this functionality. 
This PR is in support of https://github.com/hyperledger-labs/fabric-token-sdk/pull/478 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 17:55:15 +0000 UTC
    </div>
</div>

