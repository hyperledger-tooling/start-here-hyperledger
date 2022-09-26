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
                PR <a href="https://github.com/hyperledger/solang/pull/1024" class=".btn">#1024</a>
            </td>
            <td>
                <b>
                    constant overflow compatible with solc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR evaluates expressions constant arithmetic and checks for overflow according to what Solc does

Signed-off-by: salaheldinsoliman <salaheldin_sameh@aucegypt.edu>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 11:50:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1023" class=".btn">#1023</a>
            </td>
            <td>
                <b>
                    Create switch instruction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We aim at moving the dispatch code to codegen. It means we'll need new instructions and builtin structs there, like the `switch` instruction, utilized in [this line](https://github.com/hyperledger/solang/blob/6083938df34d288ba85a19d72338ee5abcb85b85/src/emit/dispatch.rs#L103).

This PR wires up the `switch` instruction for that and enables the code generation for switch statements in Yul, using the newly added instruction.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 04:02:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1022" class=".btn">#1022</a>
            </td>
            <td>
                <b>
                    Substrate: Remove seal_tombstone_deposit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">substrate</span>
            </td>
            <td>
                This API call does no longer exist in `ink!`

It looks like I changed the tests but that is only because of git is trying to be smart. I simply deleted the test for this API call and renamed the other ones to fill the gap.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 12:58:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1021" class=".btn">#1021</a>
            </td>
            <td>
                <b>
                    On Solana, stack allocations must happen in the first block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                If not, the Solana llvm target will fail to generate code with the error:

Unsupported dynamic stack allocation on create_program_address

Fixes https://github.com/hyperledger/solang/issues/1019

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 09:01:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1020" class=".btn">#1020</a>
            </td>
            <td>
                <b>
                    Update issue templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add template for new issues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 14:22:31 +0000 UTC
    </div>
</div>

