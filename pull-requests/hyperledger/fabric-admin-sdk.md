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

