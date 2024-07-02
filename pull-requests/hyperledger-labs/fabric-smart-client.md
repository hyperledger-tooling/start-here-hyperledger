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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    Support for traces
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
        Created At 2024-07-02 17:49:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    improve logs
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
        Created At 2024-07-02 15:11:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    fabric-sdk: refactor generic's peer manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 14:28:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/609" class=".btn">#609</a>
            </td>
            <td>
                <b>
                    fabric: inject drivers into provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the need to have global fabric drivers. Now the drivers are injected directly into the provider.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 13:11:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    endorser service
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
        Created At 2024-07-02 13:11:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    Support for Orion deployment
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
        Created At 2024-07-02 11:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/606" class=".btn">#606</a>
            </td>
            <td>
                <b>
                    check if grpc server is nil before accessing it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                caused panic if `grpc.enabled: false`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 10:21:34 +0000 UTC
    </div>
</div>

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

