---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/710" class=".btn">#710</a>
            </td>
            <td>
                <b>
                    fixes #708 : ca enrollments should be made with the ROOT CA cert
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses Issue #708 

For older versions of cURL, the client was accepting the NODE TLS certificate when connecting to a service endpoint.

In modern cURL / libcURL, the client places additional constraints on the server certificate, and will refuse to accept a self-signed certificate unless the root CA has been installed in the certificate bundle.

The update in this case is to present the ROOT TLS certificate when connecting to the CA using cURL. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 15:28:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/709" class=".btn">#709</a>
            </td>
            <td>
                <b>
                    Java erc721 token standard chaincode implementation.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Java chaincode for ERC721 NFT standrad. It follows the same logic as the exiting golang and Javascript implementation in the repo.

Signed-off-by: renjithpta <renjithkn@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 13:47:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    FAB-00000 Enrich test net docs.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add network diagram and Docker network container table.

This makes understanding the test network easier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-03 01:28:56 +0000 UTC
    </div>
</div>

