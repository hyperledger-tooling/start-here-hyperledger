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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1243" class=".btn">#1243</a>
            </td>
            <td>
                <b>
                    Bugfix: Struct with fields of BytesN types can not be encoded with memcpy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes an encoding bug: When a struct has any field with `BytesN` type, this field requires an endianess swap and can't be encoded or decoded directly (e.g. with a `MemCopy`).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 11:48:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1242" class=".btn">#1242</a>
            </td>
            <td>
                <b>
                    Improve code as suggested by clippy -W clippy::pedantic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                clippy::pedantic can come up with some good suggestions. Implement some of them; there are more to be done.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 10:38:15 +0000 UTC
    </div>
</div>

