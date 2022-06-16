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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/869" class=".btn">#869</a>
            </td>
            <td>
                <b>
                    Fix clippy warnings when using upcoming rust 1.62
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                rust 1.62 will be released on the 30th of June. This PR fixes the clippy warnings that will appear when that version is used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-12 08:40:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/866" class=".btn">#866</a>
            </td>
            <td>
                <b>
                    Submodules are now required to run tests
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
        Created At 2022-06-09 07:19:03 +0000 UTC
    </div>
</div>

