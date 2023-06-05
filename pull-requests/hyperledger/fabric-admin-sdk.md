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
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    implement parse SignaturePolicyEnvelope to human readable expression
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #127
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 08:53:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/132" class=".btn">#132</a>
            </td>
            <td>
                <b>
                    implements for PeerMembershipQuery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #125 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 06:37:18 +0000 UTC
    </div>
</div>

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

