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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Do not lose calling context in the logger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The log lines that contain the `breq` are currently missing the `req` and `httpreq` context, as well as any other calling context on that. It looks like a straight typo, that we're overwriting the `rCtx` with the constructor context of the client.
```
[2024-02-08T18:43:49.638Z] DEBUG EVMConnectorBody: {....} httpreq=dJAh7YSk pid=1 req=7hvX9eW_
[2024-02-08T18:43:49.638Z] DEBUG ==> POST https:/.../ breq=6yjJwWIC pid=1 proto=ethereum
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 20:07:15 +0000 UTC
    </div>
</div>

