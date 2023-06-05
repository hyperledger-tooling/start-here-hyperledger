---
layout: default
title: fabric-chaincode-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-node
---

# fabric-chaincode-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    Using the CLI provided gRPC configurations when starting the chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                in external mode (#318)

When utilizing the chaincode as a service, it is possible to pass some gRPC options as an argument, such as grpc.max_send_message_length. However, these server options were not utilized when declaring the server.
Resolves #318
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 14:31:11 +0000 UTC
    </div>
</div>

