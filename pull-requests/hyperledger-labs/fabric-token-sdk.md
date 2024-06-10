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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/653" class=".btn">#653</a>
            </td>
            <td>
                <b>
                    remove append from crypto library
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
        Created At 2024-06-10 14:39:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    Separate token parsing from storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                The existing implementation opens up a database transaction and then starts parsing the token request. This operation indirectly, via other structs, does a few database calls outside of the open db transaction. This causes failures when performing a large amount of concurrent transactions in specific configurations; specifically with sqlite as backend or with a low maximum of open database connections.

This PR splits out the parsing from the storing/deleting operations, to leave the db transaction open for as short as possible and free up resources again. As a bonus it improves the testability of the parsing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-10 08:58:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    Refactor integration tests and add web socket integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Split the tests into more parts
* Added web socket integration tests
* Extracted common code from integration tests to avoid duplication
* Added selectors to distinguish when we need the ID and when the name of a node
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 07:21:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    stress test + audit bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                This PR brings the following:
- An integration test that can be run locally for stress tests;
- A fix to the auditor lock strategy that avoids deadlocks that was discovered during the stress test;

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 05:12:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-04 08:03:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/648" class=".btn">#648</a>
            </td>
            <td>
                <b>
                    move types to utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cleanup</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-04 07:22:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/647" class=".btn">#647</a>
            </td>
            <td>
                <b>
                    reduce the use of view.Identity where possible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cleanup</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-04 06:47:33 +0000 UTC
    </div>
</div>

