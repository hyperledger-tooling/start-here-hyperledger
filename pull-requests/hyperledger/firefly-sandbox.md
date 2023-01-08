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
- [ ] have a strategy for websocket events of multiple namespaces

Discussions required on way of doing things:
- [ ] (discussion) Hacking the query in fetch util to add the selected namespace might not be a good idea. A better way is to pass namespace down to the components
- [ ]  (discussion) When a namespace is switched, handle necessary refreshes other than reload the whole page
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 01:20:17 +0000 UTC
    </div>
</div>

