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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    Fix mapping inside struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solang crashes when we try to access a mapping that is a member of a struct. There was a bug during code generation, in which we were not considering that struct members can be mappings. This PR should fix a problem raised in #785.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 10:53:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    cast struct member reference to wrong type causes panic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should be detected during sema.

Fixes https://github.com/hyperledger-labs/solang/issues/867
Fixes https://github.com/hyperledger-labs/solang/issues/868
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 14:45:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/879" class=".btn">#879</a>
            </td>
            <td>
                <b>
                    Using storage variables does not mean a function reads from storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A function only has to be view if it loads from storage.

Fixes https://github.com/hyperledger-labs/solang/issues/827

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 14:43:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/873" class=".btn">#873</a>
            </td>
            <td>
                <b>
                    WIP: Create test with simple auction contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Taken from https://docs.soliditylang.org/en/v0.8.3/solidity-by-example.html#voting

This test is broken in many ways. This PR is just a start.

- [ ] calling bid() fails without any useful error. Ensure that the error is presented in node (I think there is an account missing from the call)
- [ ] make bid function work
- [ ] make the withdraw function work/collecting of winnings
- [ ] deploy auction contract with PDA
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:30:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/872" class=".btn">#872</a>
            </td>
            <td>
                <b>
                    Do not re-export solang_parser from solang crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No reason re-export.

We're exporting far too much right now. This is just a simple start.

See https://docs.rs/solang/latest/solang/ for example
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:01:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/871" class=".btn">#871</a>
            </td>
            <td>
                <b>
                    Bump clap version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently CI tests are failing. Fix this
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 11:39:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/870" class=".btn">#870</a>
            </td>
            <td>
                <b>
                    Bump @solana/solidity
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
        Created At 2022-06-13 11:35:55 +0000 UTC
    </div>
</div>

