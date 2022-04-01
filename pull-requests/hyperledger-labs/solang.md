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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/716" class=".btn">#716</a>
            </td>
            <td>
                <b>
                    Integrate inline assembly to graphviz
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR integrates the YUL AST to the graphviz visualization tool. I also fixed a bug in which Solang was panicking when we used `--emit ast-dot` with an invalid contact.

Please, feel free to plot the dot files I added to the tests to check they are OK.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 18:47:07 +0000 UTC
    </div>
</div>

