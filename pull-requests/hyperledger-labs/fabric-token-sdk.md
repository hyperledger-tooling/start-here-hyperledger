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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    Test FSC version
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
        Created At 2024-06-14 08:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    DIG for tokensdk
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
        Created At 2024-06-13 12:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    endorsers
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
        Created At 2024-06-13 08:54:25 +0000 UTC
    </div>
</div>

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
                <span class="chip">cleanup</span>
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

