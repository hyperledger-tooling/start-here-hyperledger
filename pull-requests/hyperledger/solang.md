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
                PR <a href="https://github.com/hyperledger/solang/pull/1031" class=".btn">#1031</a>
            </td>
            <td>
                <b>
                    WIP: Split integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lucas Steuernagel <lucas.tnagel@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 21:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1029" class=".btn">#1029</a>
            </td>
            <td>
                <b>
                    Implement function dispatch in codegen for Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                This PR implements the function dispatch and the constructor dispatch in codegen for the Solana target. The old implementation in `src/emit/dispatch` has been moved to `src/emit/substrate/dispatch` and implemented as methods of `SubstrateTarget` because they are now Substrate specific.

There are some new instructions in the control flow graph for LLVM instructions that were exclusive to `emit`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 18:24:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1027" class=".btn">#1027</a>
            </td>
            <td>
                <b>
                    Function name mangling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implement function name mangling in sema.

I used the simplest mangling algorithm possible: I think that basically re-using the `.signature` field of the function fits our use case well here:
* It should already be unique for each function
* Return values do not matter in the distinction of overloaded functions (in solidity the arguments must still be different).
* The mangled function names are very user friendly, since they contain the name together with the argument types.

But I might be missing something here, I'm open to change this if there is a better solution.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 12:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1026" class=".btn">#1026</a>
            </td>
            <td>
                <b>
                    Use partition_point() rather than a hand-rolled linear scan
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                First, this fixes a problem in the file offset to line/column number conversion. This happens if the offset lands exactly on the newline.

Secondly, this replaces a linear scan with [partition_point](https://doc.rust-lang.org/std/primitive.slice.html#method.partition_point).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 12:13:45 +0000 UTC
    </div>
</div>

