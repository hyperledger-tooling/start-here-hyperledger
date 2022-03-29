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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/710" class=".btn">#710</a>
            </td>
            <td>
                <b>
                    Detect unused functions in inline assembly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements an algorithm to detect unused functions in YUL. I've included tests as well.

There was some refactoring due to bugs I found along the way.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 19:26:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    Add yul to unused variable detection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR integrates the YUL semantic analysis to the unused variable detection algorithm. I also remove repeated and unused code from the `sema/unsused_variable.rs` file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 19:35:43 +0000 UTC
    </div>
</div>

