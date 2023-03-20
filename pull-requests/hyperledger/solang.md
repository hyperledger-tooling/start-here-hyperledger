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
                PR <a href="https://github.com/hyperledger/solang/pull/1228" class=".btn">#1228</a>
            </td>
            <td>
                <b>
                    Integration tests: Require contract names to be unique
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
        Created At 2023-03-20 09:02:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1227" class=".btn">#1227</a>
            </td>
            <td>
                <b>
                    Add release flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `--debug` flag, that enables all debugging features of the compiler (debug prints, logging runtime errors and logging api return codes). This can be considered a shortcut to enabling all features one by one. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-19 16:12:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1226" class=".btn">#1226</a>
            </td>
            <td>
                <b>
                    Forbid encoding and decoding of recursive types in sema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This aligns Solang with solc. Also on our `main` branch, `solang compile` crashes on the added test case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 16:17:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1225" class=".btn">#1225</a>
            </td>
            <td>
                <b>
                    Be clear on Solana support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR clarify the support for Solana, as requested in #786 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 15:01:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1224" class=".btn">#1224</a>
            </td>
            <td>
                <b>
                    Treat enums as 8bit uint in constant hashing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes https://github.com/xermicus/fuzzy-sol/issues/51
Closes https://github.com/xermicus/fuzzy-sol/issues/67
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 14:47:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1223" class=".btn">#1223</a>
            </td>
            <td>
                <b>
                    Remove unused argument to parse_number
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                2nd argument to `fn parse_number()` in the lexer is not used, remove.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 13:39:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1222" class=".btn">#1222</a>
            </td>
            <td>
                <b>
                    fix compilation failure with -g flag in substrate integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes compilation error when inserting the `-g` flag in Substrate integration tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 19:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1221" class=".btn">#1221</a>
            </td>
            <td>
                <b>
                    Implement rational eval of compare, or, and, and conditional operator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are all accepted by solc so solang should do the same.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 16:45:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1220" class=".btn">#1220</a>
            </td>
            <td>
                <b>
                    Remove non-idiomatic use of LinkedList
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See the note here:

https://doc.rust-lang.org/std/collections/struct.LinkedList.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 09:23:09 +0000 UTC
    </div>
</div>

