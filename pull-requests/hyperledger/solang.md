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
                PR <a href="https://github.com/hyperledger/solang/pull/1309" class=".btn">#1309</a>
            </td>
            <td>
                <b>
                    Fix the formatting in the chain extension documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sorry for this annoyance. I should have checked it before. I just assumed because it rendered it would look fine :grin:
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 17:37:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1307" class=".btn">#1307</a>
            </td>
            <td>
                <b>
                    Read compiler configurations from toml file.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1- Refactor `solang.rs`
2- Create a Struct `Configurations`, that can be created from the command line or from a `.toml` file.
3- Create a new subcommand `solang new`, which creates a project directory that includes a solidity example `flipper.sol` and `Solang.toml`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 02:10:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1306" class=".btn">#1306</a>
            </td>
            <td>
                <b>
                    Add padding in account deserialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                According to Solana's C SDK, there is a padding between accounts: https://github.com/solana-labs/solana/blob/427ad7b5bde27fe71cff13a1ed0a6a3f26302ed4/sdk/bpf/c/inc/sol/deserialize.h#L50-L68
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 14:49:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1305" class=".btn">#1305</a>
            </td>
            <td>
                <b>
                    Implement chain extensions builtin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Provide a builtin to call chain extensions. This is the building block for implementing more high level interfaces directly in Solidity.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 14:42:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1304" class=".btn">#1304</a>
            </td>
            <td>
                <b>
                    Unbreak readthedocs build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Longer term I would like to generate the docs in github actions rather then from readthedocs. If there is a failure we would like to know about it.

So, this PR does a bunch of work to fix the docs build. Now, the correct version number is rendered.

The pdf is not generated yet. Not sure if we care about the pdf though.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 13:52:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1303" class=".btn">#1303</a>
            </td>
            <td>
                <b>
                    Add missing evm builtins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 -   Added some EVM only builtins (improves evm semantic tests)
 -  tx.origin is not payable


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 14:57:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1302" class=".btn">#1302</a>
            </td>
            <td>
                <b>
                    Using for not permitted in interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `using` does not make any sense in interfaces, as they contain no function bodies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 08:30:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1301" class=".btn">#1301</a>
            </td>
            <td>
                <b>
                    update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates some dependencies.

~~Most notably inkwell 0.2.0 which now supports LLVM 16 :eyes:~~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 13:49:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1300" class=".btn">#1300</a>
            </td>
            <td>
                <b>
                    Update substrate-contracts-node to v0.25.0
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
        Created At 2023-05-08 09:59:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1299" class=".btn">#1299</a>
            </td>
            <td>
                <b>
                    Enable tests for stdlib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces the following changes:
1. Stdlib is now build directly with `cargo build`, so all the wasm and bpf files have been removed from the repository.
2. Enable the tests for the stdlib. If nothing fails within two minutes, the test passes.
3. Enable the linter `clang-format` for the stdlib. All C files have been reformatted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 21:15:11 +0000 UTC
    </div>
</div>

