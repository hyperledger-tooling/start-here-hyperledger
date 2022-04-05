---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    chore: add missing clone derives
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
        Created At 2022-04-04 11:54:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Implement mutability check for yul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements mutability checks for YUL. We check if a pure function reads or writes the state and if a view function writes the state. I've provided tests as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 15:13:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    Remove unused parameters of recursive functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found with:

$ rustup update nightly
$ cargo +nightly clippy --tests --bins

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 09:29:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    Rename assembly to yul in Solang
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR refactors Solang Parser. We decided to adopt the name "YUL" for everything that refers to Solidity assembly, so we are changing the nomenclature everywhere.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 12:57:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    Remove printer.rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the `printer.rs` file from `src/sema` and updates the documentation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 18:07:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Implement reachable for inline assembly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the `reachable` function for the inline assembly statement.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 16:54:07 +0000 UTC
    </div>
</div>

