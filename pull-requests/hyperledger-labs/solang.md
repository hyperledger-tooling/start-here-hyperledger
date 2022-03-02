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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Updates for vscode extension 0.3.0
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
        Created At 2022-03-02 10:08:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Barcelona Release v0.1.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added
 - On Solana, the accounts that were passed into the transactions are listed in the `tx.accounts` builtin. There is also a builtin struct `AccountInfo`
 - A new common subexpression elimination pass was added, thanks to [LucasSte](https://github.com/hyperledger-labs/solang/pull/550)
 - A graphviz dot file can be generated from the ast, using `--emit ast-dot`
 - Many improvements to the solidity parser, and the parser has been spun out in it's own create `solang-parser`.
    
Changed
 - Solang now uses LLVM 13.0, based on the [Solana LLVM tree](https://github.com/solana-labs/llvm-project/)
 - The ast datastructure has been simplified.
 - Many bugfixes across the entire tree.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 15:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Add tests for msg.sender system call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes tests for the `msg.sender` system call.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 12:53:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/681" class=".btn">#681</a>
            </td>
            <td>
                <b>
                    Enable assembly compatibility on Solang parser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the Solang-parser to be compatible with inline assembly and does some refactoring.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 19:05:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/680" class=".btn">#680</a>
            </td>
            <td>
                <b>
                    Add missing cast which causes pointer to address not to be loaded
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
        Created At 2022-02-24 18:51:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/677" class=".btn">#677</a>
            </td>
            <td>
                <b>
                    Support abi.encodeCall() syntax (introduced in solc 0.8.12)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is nice syntax from solc-0.8.12 which type-checks the arguments.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 16:53:34 +0000 UTC
    </div>
</div>

