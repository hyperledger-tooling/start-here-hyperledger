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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    Correct dependency version for Java protobufs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Keep in step with transient dependencies of gRPC packages to avoid runtime version resolution issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 15:12:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Allow per-call gRPC call options in Node client
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
        Created At 2021-10-27 14:11:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    Fixup scenario tests for endorser retry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The endorser retry logic has been merged into fabric main branch.  Once the peer docker image has been uploaded, a few fabric-gateway scenario tests will fail (the error details will contain more items where more endorsements have been attempted).  This PR fixes those failures.  It doesn't add any more tests at this stage.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 14:26:13 +0000 UTC
    </div>
</div>

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
                Contributes to #198 
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

