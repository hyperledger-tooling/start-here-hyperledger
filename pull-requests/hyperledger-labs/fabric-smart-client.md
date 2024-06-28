---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/605" class=".btn">#605</a>
            </td>
            <td>
                <b>
                    allow a second registration of the same fabric driver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In our project, we have  integration tests that create two FSC nodes in a single process. It's a nice and quick way to start them. Since the new dig dependency injection, our test panics because the Fabric SDK is registered twice. This PR fixes that by just warning instead of panicking. But is this the way to go?

(Also, I'd be interested to know whether the driver registration + dig might be doing the same thing in two different ways? Do we need both?)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 14:59:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/604" class=".btn">#604</a>
            </td>
            <td>
                <b>
                    Support for traces in sessions
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
        Created At 2024-06-21 17:18:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/603" class=".btn">#603</a>
            </td>
            <td>
                <b>
                    Fixed concurrent read-write
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
        Created At 2024-06-21 15:43:37 +0000 UTC
    </div>
</div>

