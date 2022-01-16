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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/640" class=".btn">#640</a>
            </td>
            <td>
                <b>
                    feat(parser): line comments
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
        Created At 2022-01-16 15:15:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/638" class=".btn">#638</a>
            </td>
            <td>
                <b>
                    Add Location To Solidity Pragma Directive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds location to solidity pragma directive. Last part to get [flatten PR](https://github.com/gakonst/ethers-rs/pull/774) merged.

Signed -off-by: Roman Krasiuk <rokrassyuk@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 19:28:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/637" class=".btn">#637</a>
            </td>
            <td>
                <b>
                    Support skiping implicit type cast checking by using flag --no-implicit-type-cast-check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi,

I created this PR to resolve the issue reported in https://github.com/hyperledger-labs/solang/issues/632 where Solang reports errors on implicit type truncation of integers (which Solc can compile well).

In particular, I added a field `pub implicit_type_cast_check: bool` into the structure `Options` to capture this flag.

I also move the structure `Options` from `codegen/mod.rs` into `lib.rs` so that the compiler options can be accessed by both `sema` and `codegen` modules.

Can you review this PR and advise if my implementation can be merged?

Thank you!


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 09:59:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    feat(parser): missing assembly statements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger-labs/solang/issues/631
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 12:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/635" class=".btn">#635</a>
            </td>
            <td>
                <b>
                    Enable linux arm64 build on self hosted runner
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
        Created At 2022-01-10 11:10:16 +0000 UTC
    </div>
</div>

