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
                PR <a href="https://github.com/hyperledger/solang/pull/1233" class=".btn">#1233</a>
            </td>
            <td>
                <b>
                    Upgrade Anchor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR upgrades the Anchor version to v0.27.0. The IDL does not have the `state` field anymore.

The container CI image needs to be updated in https://github.com/hyperledger/solang-llvm/pull/9.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 19:10:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1232" class=".btn">#1232</a>
            </td>
            <td>
                <b>
                    Refactor accounts collection to maintain proper ordering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We are going to introduce new syntax of Solidty on Solana, that allows developers to declare account names within `@signer` and `@writer` annotations. These accounts will be accessible through `tx.accounts.account_name`, which relies on the deserialization order of accounts. 

For serialization consistency, we must care about the order in which we place accounts in the IDL file, so a refactor was necessary in `solana_accounts.rs` to account for a proper ordering.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 17:01:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1231" class=".btn">#1231</a>
            </td>
            <td>
                <b>
                    Runner test
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
        Created At 2023-03-22 12:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1230" class=".btn">#1230</a>
            </td>
            <td>
                <b>
                    Fix panic when lexing ".9" at the beginning of a file
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
        Created At 2023-03-21 14:47:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1229" class=".btn">#1229</a>
            </td>
            <td>
                <b>
                    No need for ubuntu-20.04, we can move to ubuntu-latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These jobs use containers anyway.

This also contains fixes for running on self-hosted runners, like cleanup the substrate docker container 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 08:46:30 +0000 UTC
    </div>
</div>

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
                Waiting for #1222
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
                This PR adds a `--release` flag, that disables debugging features.
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

