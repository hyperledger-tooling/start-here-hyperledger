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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    Refactor unescape function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `unescape` function in `sema/expression` could not handle escape constructs, such as `\xf4` and `\u00c3`. This PR fixes such a bug.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 11:16:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    WIP: array of structs should not be array of pointers to struct
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
        Created At 2022-03-04 09:51:10 +0000 UTC
    </div>
</div>

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

