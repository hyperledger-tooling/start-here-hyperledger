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
                PR <a href="https://github.com/hyperledger/solang/pull/1217" class=".btn">#1217</a>
            </td>
            <td>
                <b>
                    Collect the accounts a contract needs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR, we collect all accounts we can from a Solidity contract and insert them into the accounts vector for an instruction, so developers do not have to input them manually.

Closes #1191.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 18:38:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1214" class=".btn">#1214</a>
            </td>
            <td>
                <b>
                    Use named enums for a few cfg expressions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make the More, Less, MoreEqual, LessEqual cfg expression named. Also Replace Expression::SignedMore and UnsignedMore with a single expression enum. This should make it more consistent.

Note for CSE we now have consistent handling for Less and LessEqual wrt signedness. I am not sure this fixes any bugs, but it makes the code consistent/readable.

Fixes #1200 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 11:41:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1213" class=".btn">#1213</a>
            </td>
            <td>
                <b>
                    solang-parser README.md should mention breaking changes may occur
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update README.md to indicate that breaking changes could occur at any time.

Fixes #1212
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 13:37:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1211" class=".btn">#1211</a>
            </td>
            <td>
                <b>
                    Refactor scale decoder into codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Decoding for `abi.decode` is now done in codegen. Like with the encoder, most of the code can be shared with the borsh decoder.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-04 21:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1210" class=".btn">#1210</a>
            </td>
            <td>
                <b>
                    Remove unnecessary files from solang crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These files bloat the crate file without any function. The list of files can be seen with `cargo package --list`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1209" class=".btn">#1209</a>
            </td>
            <td>
                <b>
                    Bump solang-parser version for crate publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note we don't want to include the entire solc source tree in the crate, so exclude all the testdata.

New version is required for `forge fmt`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 14:00:00 +0000 UTC
    </div>
</div>

