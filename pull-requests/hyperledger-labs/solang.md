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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/925" class=".btn">#925</a>
            </td>
            <td>
                <b>
                    Fix parsing of `uint x = 1 /** foo */ + 2;`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                DocComments should not be stored in the parse tree.

There are two commits, the first fixes an issue with  the existing doccomment parsing (and adjusts the test results).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 11:55:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    Improve slice support and add `create_program_address()` solana builtin
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
        Created At 2022-07-18 08:09:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    Refactor strength reduce
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In my Borsh Encoding PR #906, strength reduce was overflowing the stack for some complex encoding cases. This PR decreases the stack size from 2KB to 768 bytes for the `reaching_values` function and from 9KB to 800 bytes for the `expression_values` function.

This PR also includes a refactoring in the strength reduce files.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 18:45:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    Do not resolve the arguments to overloaded functions/event emit twice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This covers to overloaded functions, constructors, methods, and event emit.

This solves some issues wrt to slice support which is covered in a future PR.

Fixes #779 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 08:20:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    Refactor size_of function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The function `Type::size_of` is currently only used for calculation how much size a type occupies in storage. We do not utilize it to estimate the size of an item in the memory. This PR updates the function's name to properly represent what it returns and updates its description to encourage proper usage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 15:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/918" class=".btn">#918</a>
            </td>
            <td>
                <b>
                    Fix load of vector of strings from storage on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Loading a vector of strings from storage was not working correctly. When we accessed the first element of the loaded array, we would get the wrong length, and consequently the wrong string. This PR fixes this problem.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 13:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    Add Cyrill to maintainers list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also quickly made the github handles clickable :upside_down_face: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 11:23:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/914" class=".btn">#914</a>
            </td>
            <td>
                <b>
                    Documentation: Clarify that mock VM implementations may omit aspects …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …not mattering in unit tests

As discussed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 10:29:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    Fix vscode extension build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Looks like @types/vscode 1.69.0 is broken. Do not use this version.

vscode-test has been renamed to @vscode/test-electron, update this too.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 09:10:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/912" class=".btn">#912</a>
            </td>
            <td>
                <b>
                    Support length for storage strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for retrieving the length of a string saved in storage. I implemented this to help me debug an issue with Borsh Encoding.

Solc does not support this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 20:19:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/911" class=".btn">#911</a>
            </td>
            <td>
                <b>
                    Update seal debug message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `seal_println` runtime function was superseded by `seal_debug_message` in Substrate v3.0. This PR makes the `print("...")` builtin work again for current Substrate versions.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 13:31:08 +0000 UTC
    </div>
</div>

