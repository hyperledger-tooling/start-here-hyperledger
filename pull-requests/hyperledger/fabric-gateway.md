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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    Use interface instead of @grpc/grpc-js Client class in public API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the gRPC Client is a concrete class, changes to private members can cause version-to-version type incompatibilities if the caller has a dependency on a different version of @grpc/grpc-js. Requiring an interface containing only public methods of the gRPC Client class avoids these issues, provided there are no breaking changes in the gRPC Client API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 15:08:45 +0000 UTC
    </div>
</div>

