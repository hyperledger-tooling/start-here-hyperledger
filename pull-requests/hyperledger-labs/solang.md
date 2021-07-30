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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    Improve ast printer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 17:26:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    Update for rust 1.54.0 clippy
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
        Created At 2021-07-29 21:33:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    Cleanup sema/codegen separation, improve mutability/visibility checks on override
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 10:39:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    Split sema expression into smaller function to reduce stack usage
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
        Created At 2021-07-28 14:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    Reduce the stack frame on the Solana bundle and modifier fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Turns out, the llvm does not take lifetime into consideration when
creating stack frames. All the stack space created with alloca is just
bundled into a single mega stack frame. Unfortunately, this is limited
to 4096 bytes and if the stack frame is larger, then you will get access
violation errors.

The solang_dispatch() function contained the dispatch for every function
in every contract. The dispatch includes the abi decoding; so, split
this into per-contract dispatch.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 21:15:52 +0000 UTC
    </div>
</div>

