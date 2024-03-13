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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    check for nil right away
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                it created a nil pointer panic when trying to access tok.Type
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 08:59:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    identity service refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR refactors the identity service to bring clarity to the concepts of Long-Term identity, Identity Provider, Role, and Wallet.

A long-term identity is an identity that carries a long-term unique identifier. 
Long-term identities are grouped in roles. The Token-SDK supports 4 roles: Issuers, Owners, Auditors, and Certifiers.
The Identity Provider manages long-term identities.
A wallet is bound to a long-term identity and manages its pseudonyms and tokens. 
A wallet registry manages all wallets for a given role.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 12:10:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/568" class=".btn">#568</a>
            </td>
            <td>
                <b>
                    Postgres compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR improves the compatibility with postgres by fixing some bugs encountered while running a token sdk application:

-`identity_id` has non-utf8 characters which is not supported in a `TEXT` column by postgres.
- `raw` cannot be the primary key for params if the params are too large. This PR changes the primary key to the time stored in the database, which is also unique.
- postgres does not have `ON CONFLICT REPLACE` on columns
- the 'restore auditor db' feature was doing writes while iterating over the dbentries, which causes a deadlock with a single threaded KVS.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-10 17:55:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    Test new FSC version
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
        Created At 2024-03-08 14:53:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/566" class=".btn">#566</a>
            </td>
            <td>
                <b>
                    documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is meant to add and refine the available documentation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 08:27:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/565" class=".btn">#565</a>
            </td>
            <td>
                <b>
                    unifiied db
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
        Created At 2024-03-07 12:24:39 +0000 UTC
    </div>
</div>

