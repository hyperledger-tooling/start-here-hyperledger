---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/603" class=".btn">#603</a>
            </td>
            <td>
                <b>
                    driver cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following: It refactors the `TokenManagerService` to avoid interface imports.
This makes more modular the implementation of a new driver.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 06:37:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/602" class=".btn">#602</a>
            </td>
            <td>
                <b>
                    core logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following: It removes from the `core` package the package level logging to introduce struct level logging.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 10:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/601" class=".btn">#601</a>
            </td>
            <td>
                <b>
                    network service cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following:
- Remove finality API from network service
- Cleanup ValidationCode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 08:33:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/600" class=".btn">#600</a>
            </td>
            <td>
                <b>
                    add atomic write to ttxdb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                if this is ok, we can do the same for the auditdb and remove the functions that are now on the AtomicWrite (as well as the 'txn' field) from the database struct.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 07:41:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/599" class=".btn">#599</a>
            </td>
            <td>
                <b>
                    Centralize database initialization logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simplifies opening of SQL databases by centralizing the configuration in the database package, similar to how identitydb was already doing it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 10:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/598" class=".btn">#598</a>
            </td>
            <td>
                <b>
                    append tokens on finality event
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
        Created At 2024-04-11 13:59:42 +0000 UTC
    </div>
</div>

