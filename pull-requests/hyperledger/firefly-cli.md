---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/222" class=".btn">#222</a>
            </td>
            <td>
                <b>
                    Allow contract constructor params
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I think when the fabric and ethereum commands were split out the argument checking became too strict and prevent the "params" JSON header from being set to anything other than an empty array. For smart contracts with constructors that take parameters this means you can't provide the vars needed at deploy time.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 19:09:40 +0000 UTC
    </div>
</div>

