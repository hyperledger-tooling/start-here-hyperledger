---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Fix image not found issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is an issue with building docker
`ERROR: failed to solve: golang:1.21-buster: docker.io/library/golang:1.21-buster: not found`

https://github.com/hyperledger/firefly-ethconnect/actions/runs/7579131739/job/20642836640

Fixed it by using 1.21-alpine3.19 as for example for https://github.com/hyperledger/firefly-tezosconnect/pull/34
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 10:55:04 +0000 UTC
    </div>
</div>

