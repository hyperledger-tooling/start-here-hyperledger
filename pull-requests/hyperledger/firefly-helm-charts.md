---
layout: default
title: firefly-helm-charts
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-helm-charts
---

# firefly-helm-charts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-helm-charts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-helm-charts/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    [0.6.0] EVMConnect StatefulSet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Workings towards support for FireFly v1.1.x as part of the v0.6.0 chart release, this PR adds support for the new [firefly-evmconnect](https://github.com/hyperledger/firefly-evmconnect) runtime.

Similar to the original `ethconnect` support, this will have the chart deploy `evmconnect` off to the side of FireFly (for now) as a `StatefulSet`. Persistent storage is used for `leveldb`. Unlike the `ethconnect` support, this attempts to offer greater flexibility and allow for a user to somewhat safely configure all of the EVMConnect's [config options](https://github.com/hyperledger/firefly-evmconnect/blob/main/config.md).

Integrating EVMConnect into FireFly's own config will be handled in a separate follow-up PR, where FireFly v1.1.x is supported with the new config format related to [namespace isolation](https://github.com/hyperledger/firefly-fir/pull/12).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 02:08:14 +0000 UTC
    </div>
</div>

