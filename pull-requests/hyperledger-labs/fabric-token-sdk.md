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
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/524" class=".btn">#524</a>
            </td>
            <td>
                <b>
                    allow empty prefix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Table prefixes for the sql driver are useful for data segregation if you have multiple instances of the token sdk running with different configuration / owner wallets and want to connect them to the same database instance (e.g. to save cost or ease operations in a non-production environment).

The current code defaults to an empty prefix if the tablePrefix configuration is not set, but then fails because the regex does not allow an empty prefix. This PR fixes that, so that the user can not set the tablePrefix if they don't need it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 12:12:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/523" class=".btn">#523</a>
            </td>
            <td>
                <b>
                    refactoring services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                This PR does the following: 
- Refactors the package `services/vault`. The goal is to allow different implementations of the token vault.
- Make TransactionInfoProvider private
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 10:43:09 +0000 UTC
    </div>
</div>

