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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/263" class=".btn">#263</a>
            </td>
            <td>
                <b>
                    Set default timeouts in Java samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 14:54:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    Default timeouts in Java API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The existing Node SDK has configurable default timeouts for query (evaluate), endorse and submit (submit and commitStatus), so I think having configurable defaults timeouts for each gRPC service invocation is the right thing to do. Some service invocations are likely to take significantly longer than others, and the time the client is prepared to wait for different invocations is likely to vary significantly too, so I don't think there is a good default timeout value that covers all cases.

I would really like to have made use of the gRPC **CallOptions** class directly, rather than the Fabric Gateway API having its own **CallOption** abstraction to maintain. Unfortunately the Java gRPC client stubs expect specific methods to be called for specific options (which update a **CallOptions** object internally) and don't expose a method to just specify or update the existing **CallOptions**.

Contributes to #198 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 12:28:49 +0000 UTC
    </div>
</div>

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

