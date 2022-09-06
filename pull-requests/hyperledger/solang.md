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
                PR <a href="https://github.com/hyperledger/solang/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    Fix overflow detection tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Numbers that overflow the input type was generated, causing some overflow detection tests to fail
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 21:24:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1002" class=".btn">#1002</a>
            </td>
            <td>
                <b>
                    Solana NFT example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates a Solidity contract to manage NFTs on Solana. It is an example to show Solang functionality during Solana's Singapore Hacker House. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 20:16:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    Improve vscode extension documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 13:11:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/999" class=".btn">#999</a>
            </td>
            <td>
                <b>
                    Substrate: concrete contracts must have public or external functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">substrate</span>
            </td>
            <td>
                In `ink!`, any contract must have at least one public message. This PR aligns solangs behavior up with `ink!`. It is a precondition for making #989 happen.

A public function is in a contract, if it has `public` or `external` functions, if it has a `receive` or any fallback function or if it has public storage items (those will yield public getters). A new bool flag was added to the `Contract` struct in the `sema` AST to reflect that (otherwise we need to loop through all contract functions anywhere we want to check it).
 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 12:11:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/998" class=".btn">#998</a>
            </td>
            <td>
                <b>
                    Use solang's heap implementation on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As of Solana v1.11, `sol_alloc_free_` system call is no longer available. This means that programs are expected to provide their own heap impl.

Also enable `push()` and `pop()` for memory arrays on Solana.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 12:46:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/996" class=".btn">#996</a>
            </td>
            <td>
                <b>
                    Create Solana's System Instruction library and 'solana-library' folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds to our repository a library for Solana's system instructions. They allow developers to create accounts, transfer funds and assign authorities to accounts. Creating accounts is an essential part of an NFT example on Solana created entirely with Solidity.

In addition, this PR creates a `solana-library` folder to hold all the libraries we implement for Solana.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 19:08:43 +0000 UTC
    </div>
</div>

