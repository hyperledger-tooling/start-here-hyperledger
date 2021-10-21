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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    Allow explicit timeouts for gRPC service invocations in Java API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #198 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 11:12:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    Clean up eventing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some code clean up and minimise client API implementation and behaviour beyond what is provided by gRPC.

Java:
- Use async rather than direct in-process service invocation for unit tests to better simulate runtime behaviour.
- Remove explicit closed baheviour from ChaincodeEventIterator, and let the gRPC iterator throw a gRPC error if the iterator is used after the stream is closed.
- Simplify unit test implementations.
- Simplify ChaincodeEventIterator implementation.

Node:
- Remove explicit closed behaviour from chaincode event AsyncIterable and use whatever behaviour the gRPC server stream's AsyncIterable provides.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 13:31:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Additional chaincode event close scenario tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactored use of gRPC context to close event listening to avoid interleaving of contexts and unintentional cancellation
 of gRPC calls.

Closes #213 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 17:33:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    Scenario tests for chaincode event listening close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #213 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 11:00:26 +0000 UTC
    </div>
</div>

