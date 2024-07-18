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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/709" class=".btn">#709</a>
            </td>
            <td>
                <b>
                    FSC: 418accb17b68969bf3bfa946567ec48070dd3f9c
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
        Created At 2024-07-18 06:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    Re-use logic for new wallet service
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
        Created At 2024-07-17 23:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/707" class=".btn">#707</a>
            </td>
            <td>
                <b>
                    Added PGX driver
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
        Created At 2024-07-17 23:38:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/706" class=".btn">#706</a>
            </td>
            <td>
                <b>
                    Close selector
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
        Created At 2024-07-17 23:36:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/705" class=".btn">#705</a>
            </td>
            <td>
                <b>
                    Cache Audit info
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
        Created At 2024-07-17 23:34:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/704" class=".btn">#704</a>
            </td>
            <td>
                <b>
                    Balance view
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
        Created At 2024-07-17 23:32:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/703" class=".btn">#703</a>
            </td>
            <td>
                <b>
                    Token fetcher implementations and token query optimizations to reduce…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … the amount of the data queried
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 23:17:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/701" class=".btn">#701</a>
            </td>
            <td>
                <b>
                    Update FSC version
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
        Created At 2024-07-17 12:52:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    TokensDB: Support for update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit does the following: When deleting a token, if the token does not exists, an entry in the tokens table is added and marked as deleted. When the token is later added, the entry is updated
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 12:10:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    hide pkcs11 behind a build tag so that token sdk is pure go by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Companion PR to https://github.com/hyperledger-labs/fabric-smart-client/pull/621.

Goal is to make HSM support 'opt-in' by using a build tag: `CGO_ENABLED=1 go build -tags pkcs11`. If you don't supply the tag, it will not require CGO. This makes it easier to have cross-platform builds or to use alpine containers, for instance.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 09:34:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Next commits
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
        Created At 2024-07-16 22:15:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    Updated FSC version
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
        Created At 2024-07-16 11:23:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    add config flag for retries for selectors
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
        Created At 2024-07-15 15:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    fix data race in local membership
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevent some data race for the function `GetDefaultIdentifier` (reading list of resolvers) when called from `mapStringToID`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 13:49:20 +0000 UTC
    </div>
</div>

