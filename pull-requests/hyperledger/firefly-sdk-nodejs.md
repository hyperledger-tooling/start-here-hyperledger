---
layout: default
title: firefly-sdk-nodejs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-sdk-nodejs
---

# firefly-sdk-nodejs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-sdk-nodejs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sdk-nodejs/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Allow custom app logic to trigger when a websocket connects/reconnects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When using an ephemeral WebSocket to listen for completion of a FireFly action, you need to know the socket is connected before you submit the action. This isn't currently possible in the SDK.

It's also not possible to send custom commands over the WebSocket, or trigger other processing as a side-effect of a reconnect.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 02:41:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sdk-nodejs/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    use correct options object for baseURLs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use the correct option defaults for baseURLs
- Extra check for websocket host
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 13:09:13 +0000 UTC
    </div>
</div>

