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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    Add error handling to gateway samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Shows how to access the error details in the 3 SDK samples

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 14:35:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    Samples for real-time event listening
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Augments the existing replay event listening examples.
- Includes correct close of eventing when listening is completed.
- Better examples in API documentation.

Contributes to #231 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 18:35:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    Simplify cancel impementation for Java chaincode events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #231 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 10:47:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    Stop event listening in Node client using async iterable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a close() method to the AsyncIterable returned when getting chancode events.

Contributes to #213
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 16:35:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    Rename EndpointError to ErrorDetail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The gateway proto message EndpointError was renamed to ErrorDetail and the associated changes were also made in the fabric gateway server code.
This commit renames all refererences to this in the client SDKs

Resolves https://github.com/hyperledger/fabric/issues/2971

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 14:23:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Add Transaction class description to JavaDoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also for clarity, add some spacing to async submit example in Contract JavaDoc.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 09:13:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    Generate a new transaction ID for every proposal in Java API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Calling Proposal.Builder.build() multiple times on the same builder instance will similarly configured transaction proposals, but with different transaction IDs (and channel header timestamps).

Resolves #234 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 14:44:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    Scenario tests for error paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing that errors that get raised in the peer or chaincode get reported back to the client, including details of which endorser raised the error.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 09:05:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/231" class=".btn">#231</a>
            </td>
            <td>
                <b>
                    Stop receiving chaincode events in Java API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a close() method to the event iterator that can be called when events are no longer required.

Calling close() on the event iterator cancels the server streaming gRPC connection from the client end. This requires the use of the async gRPC stub, which is significantly more complex to use than the blocking API. This complexity is hidden within a new internal GatewayClient class, which decouples the rest of the client code from the gRPC API calls.

Contributes to #213
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 13:43:04 +0000 UTC
    </div>
</div>

