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
                PR <a href="https://github.com/hyperledger/solang/pull/1254" class=".btn">#1254</a>
            </td>
            <td>
                <b>
                    Unify `external_call` and `create_contract` on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `create_contract` and `external_call` have basically the same meaning on Solana, so I united the functions we have in `solana.c`.

This is part of my task to improve the account management on Solana. Please, read my task list #1251 To understand what I am trying to achieve.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 20:52:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1253" class=".btn">#1253</a>
            </td>
            <td>
                <b>
                    chore(ci): update github actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 18:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1252" class=".btn">#1252</a>
            </td>
            <td>
                <b>
                    Fix VariableDefinition Display impl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `pt::VariableDefinition` was missing a test case so a bug wasn't caught (missing whitespace when attributes are present) in #1237
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 12:05:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1250" class=".btn">#1250</a>
            </td>
            <td>
                <b>
                    Use `wasm-tools` instead of `parity-wasm`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The API of `wasm-tools` is quite different; `wasmparser` doesn't allow to modify the blob in-place. Instead, now we iterate over the sections and manually craft any section needing changes. 

Closes #1240
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 17:31:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1249" class=".btn">#1249</a>
            </td>
            <td>
                <b>
                    Refactor substrate dispatcher into codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Implement the dispatch logic in codegen
* Remove `Instr::AbiDecode`
* Remove ABI encoding and decoding interfaces from `TargetRuntime`
* Remove `substrate.c` from the stdlib
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 12:27:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1247" class=".btn">#1247</a>
            </td>
            <td>
                <b>
                    Update substrate contracts-ci-linux docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                They were deleted from docker hub (it was not known we still use them)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 18:53:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1246" class=".btn">#1246</a>
            </td>
            <td>
                <b>
                    Pass by value types narrower than 8-bytes as suggested by `clippy::pedantic`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clippy pedantic suggests that we pass by value types narrower than 8 bytes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 17:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1245" class=".btn">#1245</a>
            </td>
            <td>
                <b>
                    Remove --math-overflow flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1216
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 16:45:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1244" class=".btn">#1244</a>
            </td>
            <td>
                <b>
                    Bugfix: Unwrap user types while processing WriteBuffer instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                User types can wrap `bytesN` which need an endianess swap during encoding.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 08:06:36 +0000 UTC
    </div>
</div>

