---
layout: default
title: firefly-sandbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-sandbox
---

# firefly-sandbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-sandbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-sandbox/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    udpate sandbox UI to support mult-namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>

Todos:

- [ ] Pick up https://github.com/hyperledger/firefly-sdk-nodejs/pull/59 & https://github.com/hyperledger/firefly-sdk-nodejs/pull/58 
- [x] have a strategy for websocket events of multiple namespaces

inputs are welcome on whether the following two logic are good enough:
- [ ] (discussion) currently the code add the query with namespace to all rest request in fetch util.
- [ ]  (discussion) When a namespace is switched, a page reload is triggered.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 01:20:17 +0000 UTC
    </div>
</div>

