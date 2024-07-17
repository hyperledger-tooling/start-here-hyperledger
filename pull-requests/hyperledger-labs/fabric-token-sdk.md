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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    orion update
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
        Created At 2024-07-10 17:25:14 +0000 UTC
    </div>
</div>

