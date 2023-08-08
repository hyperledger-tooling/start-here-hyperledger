---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1478" class=".btn">#1478</a>
            </td>
            <td>
                <b>
                    Fix incorrect deserialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The deserialization of `struct TokenAccountData` in the Solana library is incorrect. This PR fixes the issue and tests the deserialization of both `struct TokenAccountData` and `struct MintAccountData`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 21:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1476" class=".btn">#1476</a>
            </td>
            <td>
                <b>
                    Link to the Solana getting started guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1475.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 08:02:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1474" class=".btn">#1474</a>
            </td>
            <td>
                <b>
                    Represent contracts by their program id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR changes the inner representation of Solana contracts from their data account to their program id.
All the changes are listed here: https://github.com/hyperledger/solang/issues/1430

Constructors will still require an account to be initialized, even if the contract has no storage variables and no function requires a data account. This setting does not influence the overall functionality of Solang, but it is something we must solve as I have described in #1480 .

There are small changes in Polkadot tests, because I found the mutability check to be incomplete. We were not recursing down all expressions, so reads and writes from the state went unnoticed. I fixed this as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 20:24:06 +0000 UTC
    </div>
</div>

