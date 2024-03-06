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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/564" class=".btn">#564</a>
            </td>
            <td>
                <b>
                    identity stack cleanup
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
        Created At 2024-03-05 08:43:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/563" class=".btn">#563</a>
            </td>
            <td>
                <b>
                    remove suffix, use prefixes consistently, only rollback on error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We don't need the tablesuffix because the db is configured by the user per TMS. Even if they choose to use the same database for multiple TMS, they can use the prefix to have different tables per TMS.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-03 15:11:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/562" class=".btn">#562</a>
            </td>
            <td>
                <b>
                    identity types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following: replace the `SerializedIdentity` type with more specific identity types.
This allows a driver to support multiple owner identity types
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-03 10:35:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/561" class=".btn">#561</a>
            </td>
            <td>
                <b>
                    self-contained identity stack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                See #558 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 11:09:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/560" class=".btn">#560</a>
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
                This PR proposes the following:
- remove transient-related function from the network service, they are not needed anymore
- cleanup sql db logs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 10:16:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/557" class=".btn">#557</a>
            </td>
            <td>
                <b>
                    `tokendb` and `tokens`'s support for transactions
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
        Created At 2024-02-28 14:57:20 +0000 UTC
    </div>
</div>

