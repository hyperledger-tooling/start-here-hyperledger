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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    Extract cache
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
        Created At 2024-04-30 13:31:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    add test for query token details
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
        Created At 2024-04-29 16:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    check status and tokens from the dbs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR reduces to the minimum the use of the backend vault to check the status of a transaction.
This status must be asked to either the ttxdb or auditdb.

This PR contains also some refactoring around the vault structs and interfaces.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 14:51:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    fabric commit processor doesn't handle anymore tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This job is left to the audit and transaction dbs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 14:20:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    Reduce SP usage
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
        Created At 2024-04-26 13:55:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Update FSC
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
        Created At 2024-04-25 15:37:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    get datasource from environment variable, fix panic on open db error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 13:51:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Fts crypto code refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Remove un-necessary crypto code. 
* Remove anonymous issuance for the time being. Replace it instead with `type_is_hidden` or `not`. In systems with a single issuer hiding the type can be required. For transparent accounting, systems may require the type to be revealed at issuance time. In systems where a single issuer issues a single type, the type is implicitly revealed. 
* We plan to support anonymous issuance if applications call for it. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 09:23:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/614" class=".btn">#614</a>
            </td>
            <td>
                <b>
                    query directly token requests
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
        Created At 2024-04-25 05:46:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    remove orion commit processor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does the following: It removes the orion transaction processor. Transactions are committed into the local databases upon an event received via a finality listener. 
Next step is to remove the fabric transaction processor too. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 04:14:50 +0000 UTC
    </div>
</div>

