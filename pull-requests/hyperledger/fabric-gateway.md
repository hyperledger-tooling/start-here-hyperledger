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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    Fix bad unit test for CommitStatus error in Go client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The error handling is also wrong and wasn't picked up because of the bad unit test.

Resolves #158
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 08:15:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/159" class=".btn">#159</a>
            </td>
            <td>
                <b>
                    Return gRPC errors directly in Go client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Avoid wrapping errors to allow client applications to interrogate gRPC status and additional details associated with the error.

Resolves #158
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 17:42:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    go hsm signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 09:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/156" class=".btn">#156</a>
            </td>
            <td>
                <b>
                    Example of reading ids from JSON files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two main types of JSON file that contain ids. Example of reading those and then prcoessing them for use with the gateway

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 15:57:40 +0000 UTC
    </div>
</div>

