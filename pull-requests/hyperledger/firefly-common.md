---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Support custom dispatchers for event streams
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have a use of this library, where I need to handle events within the Go code directly - using constructs specific to the Microservice.

Unlike the Webhook and WebSocket implementations, these cannot be made generic in the common library. So instead, I propose adding this extension point to the common library to allow me to extended it with my implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-02 20:52:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    Add error return to query modifier
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
        Created At 2024-01-01 00:12:25 +0000 UTC
    </div>
</div>

