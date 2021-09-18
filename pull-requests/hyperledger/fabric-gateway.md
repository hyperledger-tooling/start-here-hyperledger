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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Provide enumeration of commit status codes in Node client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows client applications to interpret the numeric status code values and check them against specific values of interest.

Note the scenario test change, which demonstrates how commit status values can be referenced by client application code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-18 12:26:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Use accessors for protobuf fields in Go client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using getters to access fields on protobuf structs reduces the chance of runtime panics in the event that malformed protobuf messages are received from the Fabric Gateway peer. Results returned to the application will still not be correct but the chance of application failure is reduced.

Note: this is **not** a fix for #193 but may make diagnosis of bugs of this type easier in the Go client, since the client is more likely to remain running for debugging or results analysis.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 13:24:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Check for null names in Java client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Network name in Gateway.getNetwork()
- Chaincode ID in Network.getContract() and Network.getChaincodeEvents()
- Transaction name in Contract.submitTransaction(), evaluateTransaction() and newProposal()
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 15:14:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Expose ChaincodeEventsRequest as interface in Java API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Consistency with other classes that implement behaviour.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 11:29:39 +0000 UTC
    </div>
</div>

