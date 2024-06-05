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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/646" class=".btn">#646</a>
            </td>
            <td>
                <b>
                    db extensions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR introduces a mechanism to extend the TokenDB to store additional information about a token. 
For example, when a token's owner field contains an HTLC (`service/interop/htlc`) script, it would be convenient to store script-related information for more targeted queries and data analysis.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-02 07:43:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/645" class=".btn">#645</a>
            </td>
            <td>
                <b>
                    remove storage service as it is not needed anymore
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
        Created At 2024-06-02 07:42:39 +0000 UTC
    </div>
</div>

