---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-dataexchange-https/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Setting a Default Request Timeout for REST API Calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing FireFly DX in an env with a bad network, I noticed DX would "hang" for roughly 2m10s on each req attempt until `ETIMEDOUT` was thrown:
```
2021-12-09T18:41:37.758Z [INFO ]: FireFly Data Exchange running on http://0.0.0.0:5000 (API) and https://0.0.0.0:5001 (P2P) - log level "DEBUG" app.ts
2021-12-09T18:42:06.511Z [INFO ]: New WebSocket client connected (client count: 1) app.ts
2021-12-09T18:42:06.511Z [INFO ]: New WebSocket delegate assigned app.ts
2021-12-09T18:44:36.353Z [DEBUG]: post https://firefly-dx.example.com/api/v1/messages utils.ts
2021-12-09T18:46:46.263Z [ERROR]: post https://firefly-dx.example.com/api/v1/messages attempt 0 [undefined] Error: connect ETIMEDOUT 10.1.6.180:443
    at TCPConnectWrap.afterConnect [as oncomplete] (net.js:1159:16) utils.ts
2021-12-09T18:46:46.765Z [DEBUG]: post https://firefly-dx.example.com/api/v1/messages utils.ts
2021-12-09T18:48:57.334Z [ERROR]: post https://firefly-dx.example.com/api/v1/messages attempt 1 [undefined] Error: connect ETIMEDOUT 10.1.6.180:443
    at TCPConnectWrap.afterConnect [as oncomplete] (net.js:1159:16) utils.ts
2021-12-09T18:48:57.836Z [DEBUG]: post https://firefly-dx.example.com/api/v1/messages utils.ts
2021-12-09T18:51:08.406Z [ERROR]: post https://firefly-dx.example.com/api/v1/messages attempt 2 [undefined] Error: connect ETIMEDOUT 10.1.6.180:443
    at TCPConnectWrap.afterConnect [as oncomplete] (net.js:1159:16) utils.ts
2021-12-09T18:51:08.907Z [DEBUG]: post https://firefly-dx.example.com/api/v1/messages utils.ts
2021-12-09T18:53:19.478Z [ERROR]: post https://firefly-dx.example.com/api/v1/messages attempt 3 [undefined] Error: connect ETIMEDOUT 10.1.6.180:443
    at TCPConnectWrap.afterConnect [as oncomplete] (net.js:1159:16) utils.ts
2021-12-09T18:53:19.979Z [DEBUG]: post https://firefly-dx.example.com/api/v1/messages utils.ts
2021-12-09T18:55:30.550Z [ERROR]: post https://firefly-dx.example.com/api/v1/messages attempt 4 [undefined] Error: connect ETIMEDOUT 10.1.6.180:443
    at TCPConnectWrap.afterConnect [as oncomplete] (net.js:1159:16) utils.ts
2021-12-09T18:55:31.051Z [INFO ]: Event emitted message-failed/2962a5f9-d6b6-4d19-9746-2dfedc054d1e app.ts
2021-12-09T18:55:31.052Z [ERROR]: Failed to deliver message Error: connect ETIMEDOUT 10.1.6.180:443 handlers/messages.ts
```

According to https://github.com/axios/axios/issues/1739 and https://axios-http.com/docs/req_config, setting this should make it so these reqs fail much more quickly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 19:14:51 +0000 UTC
    </div>
</div>

