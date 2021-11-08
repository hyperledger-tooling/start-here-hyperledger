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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/301" class=".btn">#301</a>
            </td>
            <td>
                <b>
                    Rename the root json config file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the releasing notes

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 11:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    Chaincode errors should be returned as COMPLETED
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Node shim differs from the Go shim in that returns any chaincode generated errors as grpc errors.
In Go, it just returns the ProposalResponse message with a status 500 code and error message embedded in it.
This difference makes it hard to write consistent error handling code in Fabric (esp Gateway) and the SDKs.
This commit changes the Node shim error handler to behave the same as the Go shim.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 10:29:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Rename the root json config file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 10:48:19 +0000 UTC
    </div>
</div>

