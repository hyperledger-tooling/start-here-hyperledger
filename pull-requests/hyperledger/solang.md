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
                PR <a href="https://github.com/hyperledger/solang/pull/1135" class=".btn">#1135</a>
            </td>
            <td>
                <b>
                    Bump inkwell and fix clippies for upcoming rust 1.67
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - inkwell 0.1.0 has been released, which breaks the build
- rust 1.67 will be released on the 26th, fix clippies for the release

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-22 13:03:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    Add casts for yul pointer to integer conversion and vice versa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                yul allows implicit conversion of pointers to integers and vice versa.

Fixes https://github.com/xermicus/fuzzy-sol/issues/79

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 12:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    Load value before shifting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The shift operations were not loading values before creating the respective LLVM-IR instruction. This PR fixes this and closes https://github.com/xermicus/fuzzy-sol/issues/38.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 21:01:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    Fix encoder for multidimensional dynamic arrays
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The example in the tests is the one of the cases I found in which we can use two dynamic dimensions in an array. The example helped me find various bugs in the way I was treating them in the encoder. This is also going to help @xermicus with his #1128 PR.

@xermicus You can decided whether to merge this PR or incorporate the change into your PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 19:51:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    mappings and arrays can also cause recursive struct fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes https://github.com/xermicus/fuzzy-sol/issues/31
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 15:29:57 +0000 UTC
    </div>
</div>

