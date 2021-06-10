---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Add GitHub action to build and deploy Docker images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 23:20:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Update delegate logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 14:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Assumption on code of another delegate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
{"name":"app.ts","hostname":"206b07def762","pid":1,"level":30,"msg":"Data exchange running on http://0.0.0.0:3000 (API) and https://0.0.0.0:3001 (P2P) - log level \"info\"","time":"2021-06-09T13:15:17.771Z","v":0}
/firefly-dataexchange-https/build/app.js:104
        webSocket.on('message', (message) => __awaiter(void 0, void 0, void 0, function* () {
                  ^
TypeError: Cannot read property 'on' of undefined
    at assignWebSocketDelegate (/firefly-dataexchange-https/build/app.js:104:19)
    at WebSocket.<anonymous> (/firefly-dataexchange-https/build/app.js:119:13)
    at WebSocket.emit (events.js:388:22)
    at WebSocket.emitClose (/firefly-dataexchange-https/node_modules/ws/lib/websocket.js:198:10)
    at Socket.socketOnClose (/firefly-dataexchange-https/node_modules/ws/lib/websocket.js:895:15)
    at Socket.emit (events.js:376:20)
    at TCP.<anonymous> (net.js:673:12)
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 13:36:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Optimize Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 13:03:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    Build from source tree
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I believe the docker build should be building the local source tree, rather than master from Git, but I'm not 100% sure if that's the architecture of the builds.
So copying in @nguyer for a review.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 12:51:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Second reference to certificate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 12:40:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Add option to override p2p endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 01:21:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Update label
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 22:16:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Update host
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 19:25:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Add Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 19:21:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Return error, and consistency in naming
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couple of suggestions as I've been working through the API
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 05:48:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Auto assign request ID if not present
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 01:12:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Auto generate requestID if not provided
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 01:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    Include peer endpoint in status API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-05 14:00:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    Optionally bypass API key for websocket connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-05 02:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    Introduce new features to enhance portability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Included in these changes:
 - Each organization has a unique identifier (peerID). That identifier corresponds to the combination of the `O` (organization) and `OU` (organization unit) in the certificate subject.
 - In addition to ports, hostnames are now specified for API and P2P endpoints in the configuration file.
 - New endpoint added `/id` which returns the data exchange instance peerID, P2P endpoint and certificate.
 - The API Key is now optional. If it's not included in the configuration file, the API will be accessible without having to pass the X-API-KEY header.
 - Updated samples, swagger and readme.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-05 00:18:19 +0000 UTC
    </div>
</div>

