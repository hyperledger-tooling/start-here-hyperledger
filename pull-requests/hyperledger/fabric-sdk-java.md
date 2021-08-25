---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/145" class=".btn">#145</a>
            </td>
            <td>
                <b>
                    FABJ-480 fix maxInboundMessageSize value type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add peer grpc option 'grpc.max_inbound_message_size'

relate:
[FABJ-480](https://jira.hyperledger.org/browse/FABJ-480)
[FABJ-480 fix maxInboundMessageSize yaml reading](https://github.com/hyperledger/fabric-sdk-java/pull/140)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 02:16:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Explicit dependencies in integration test chaincode (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of fc05ef2accde5956ce930623d11d5443a4d759cf from main branch.

Resolves breakages with latest releases of the chaincode shim, where more recent Gradle versions are more strict in requiring dependencies to be specified rather than picked up as transient dependencies.

Also update commons-compress dependency to address security vulnerability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 15:50:27 +0000 UTC
    </div>
</div>

