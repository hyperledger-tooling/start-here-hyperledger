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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    FABGW-21: Real-time chaincode event listening in Go API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implementation with unit test coverage of implicit signing path.

Off-line signing test coverage and scenario tests for a later PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 17:39:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    Refactor Go scenario tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Split units of functionality into different files for clarity.
- Better abstraction of Gateway connection and transaction invocation.
- Correctly initialise and clean up state before and after scenarios, including closing gRPC connections.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 11:38:08 +0000 UTC
    </div>
</div>

