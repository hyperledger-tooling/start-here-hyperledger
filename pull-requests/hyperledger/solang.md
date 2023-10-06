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
                PR <a href="https://github.com/hyperledger/solang/pull/1559" class=".btn">#1559</a>
            </td>
            <td>
                <b>
                    Fix clippy 1.73 warnings
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
        Created At 2023-10-05 22:01:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1557" class=".btn">#1557</a>
            </td>
            <td>
                <b>
                    Add function annotations 🚀
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                This PR introduces account annotations for developers to declare accounts in a Solidity function. This is one of the task items in #1251.

The new syntax tremendously facilitates writing contracts and is less error prone as we do not need to both pass the account address as an argument and in the accounts field.

I wrote some tests where I noticed they were necessary and I attempted to refactor all existing Solana Solidity to use the annotations, so that my implementation would be stress tested in all those cases.

There are a few items this PR did not accomplish, but are going to be implemented in future changes:

1. I did not validate accounts during runtime, i.e. I am not checking if the bits are properly set before dispatching the function, but I wonder if this is really needed.
2. When generating the interface for an IDL, I am not creating the account annotations, but this is an amazing feature to be added soon.
3. The `address.balance` function is useless on Solana, but has not been eliminated yet. We can now just do `tx.accounts.myAccount.lamports`.
4. The `address.send` and `address.transfer` are also not necessary, but I did not purge the compiler of them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 18:17:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1556" class=".btn">#1556</a>
            </td>
            <td>
                <b>
                    Move to github provided runners for arm macos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This means we no longer rely on the Hyperledger provided one.

See https://github.blog/2023-10-02-introducing-the-new-apple-silicon-powered-m1-macos-larger-runner-for-github-actions/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 21:12:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1555" class=".btn">#1555</a>
            </td>
            <td>
                <b>
                    update rust version to 1.72.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/solang/pull/1541 uses crate forge-fmt which depends on rust 1.72
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-01 09:42:55 +0000 UTC
    </div>
</div>

