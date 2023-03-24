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
                PR <a href="https://github.com/hyperledger/solang/pull/1236" class=".btn">#1236</a>
            </td>
            <td>
                <b>
                    Bump MSRV to 1.65
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The latest `scale-info` release requires Rust 1.65, but we are still on 1.64. I think it is fair to bump our MSRV to 1.65 since latest release is 1.68 already.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 09:25:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1235" class=".btn">#1235</a>
            </td>
            <td>
                <b>
                    Substrate: Test for instantiation nonce to increase
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Explicitly asserting the `instantiation_nonce` runtime API return value to increase after a subsequent contract deployment.

Additionally slightly cleaned up the testsuite. We can log runtime API calls in all cases, shouldn't matter. Bonus is that we no longer need to compile any test twice with adjusted settings to make this work. Also the runtime error test may not completely equal with only the error message, but this is fine we can just assert the expected runtime error to be present. It's OK if other stuff is in the debug buffer too. This makes the `runtime_errors` integration test less brittle.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 07:50:45 +0000 UTC
    </div>
</div>

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
                1- add a `--release` flag, that disables debugging features (logging prints, api return codes and runtime errors).
2- make all debugging features on by default. (make current debugging flags disable debugging)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-19 16:12:06 +0000 UTC
    </div>
</div>

