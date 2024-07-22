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
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    Multiplexer fix
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
        Created At 2024-07-22 10:11:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/635" class=".btn">#635</a>
            </td>
            <td>
                <b>
                    dispose context and close sessions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                This PR cleanups the contexts, sessions, and streams management by closing and releasing resources when needed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 03:27:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/634" class=".btn">#634</a>
            </td>
            <td>
                <b>
                    Added traces and metrics
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
        Created At 2024-07-17 11:50:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/633" class=".btn">#633</a>
            </td>
            <td>
                <b>
                    Injectable network config
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
        Created At 2024-07-17 09:55:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/632" class=".btn">#632</a>
            </td>
            <td>
                <b>
                    add closing state to prevent send on closed channel panic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With multiple subscribers and events, we encountered a race condition where the OnReceive would still try to send when CloseChaincodeEvents had already closed the channel (which causes a panic). This PR adds a unit- and integration test to reproduce it, and a `closing` boolean behind a mutex to prevent it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 08:50:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Decorator to disable histograms
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
        Created At 2024-07-16 10:50:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    Added GetOrLoad method in second chance cache
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
        Created At 2024-07-16 09:13:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Fixes for sessions
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
        Created At 2024-07-15 23:04:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Fixes
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
        Created At 2024-07-15 23:03:54 +0000 UTC
    </div>
</div>

