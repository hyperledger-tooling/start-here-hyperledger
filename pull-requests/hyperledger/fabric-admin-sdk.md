---
layout: default
title: fabric-admin-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-admin-sdk
---

# fabric-admin-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-admin-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    Update channel API for consistency with chaincode API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Callers no longer need to know about and create their own protobuf client stubs. Instead, appropriate client stubs are created using a supplied gRPC connection.
- Callers supply a Context that is used for gRPC invocations, which allows control of timeouts and cancellation of gRPC invocations. Previously invocations used context.Background() and could not be cancelled without terminating the client application.
- Parameters for functions that drive gRPC invocations are of the form `func(ctx context.Context, connection grpc.ClientConnInterface, id identity.SigningIdentity, ...)`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 13:38:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    try to impl list channel from peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #123 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 03:57:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    Ensure gRPC error details can be extracted from errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add unit tests to confirm errors returned from chaincode functions that wrap gRPC errors can have their status extracted.
- Update gRPC dependency to handle wrapped errors.

Closes #126
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 11:46:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Return result on chaincode install
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The chaincode install result includes the package ID and label for the install, which may avoid work required by the client (such as computing the package ID) in order to perform later steps in the chaincode lifecycle.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 10:11:23 +0000 UTC
    </div>
</div>

