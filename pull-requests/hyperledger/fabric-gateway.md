---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/587" class=".btn">#587</a>
            </td>
            <td>
                <b>
                    Remove Netty dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use Java gRPC instead of Netty API to establish TLS connections. Requires client application to add an appropriate gRPC channel service provider dependency, but also gives the client control of the library to be used rather than mandating Netty.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 14:33:47 +0000 UTC
    </div>
</div>

