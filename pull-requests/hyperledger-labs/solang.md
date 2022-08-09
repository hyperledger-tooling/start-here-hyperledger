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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/954" class=".btn">#954</a>
            </td>
            <td>
                <b>
                    Bug: Parse underscores in fractional component of Rational numbers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solang parser fails to parse the following valid solidity

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;
uint constant test = 1.2_3e2;
```
with the following diagnostic

```rust
Diagnostic { loc: File(0, 80, 84), level: Error, ty: ParserError, message: "unrecognised token '_3e2', expected \";\"", notes: [] }
```

This is because the Lexer doesn't include underscores in the rational part but underscores are valid https://docs.soliditylang.org/en/latest/grammar.html#a4.SolidityLexer.DecimalNumber
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 15:51:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/953" class=".btn">#953</a>
            </td>
            <td>
                <b>
                    Fix clippy warnings for upcoming rust 1.63 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                rust 1.63 should be released on the 11th of August 2022
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 13:15:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/952" class=".btn">#952</a>
            </td>
            <td>
                <b>
                    Organize installation instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I reorganized the installation instructions from our docs, making it clear that the one needs to install Solana's LLVM fork before building Solang, following the suggestion from #948.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 16:52:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/951" class=".btn">#951</a>
            </td>
            <td>
                <b>
                    Add SPDX headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Only for Rust files.

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 16:03:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/950" class=".btn">#950</a>
            </td>
            <td>
                <b>
                    Refactor builtin structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces a few changes to the builtin structs in Solang.

1. `Type::Struct(usize)` has changed to `Type::Struct(StructType)` to encompass both user defined structs and builtin structs.
2. Solana builtin structs are now held in a new data structure. We can easily retrieve their `StructDecl` data using `StructType::get_definition`. This works also for user defined structs.
3. `codegen::Expression::ExternalFunction` has been eliminated, because I replaced it by a `StructLiteral` of `Type::Struct(StructType::ExternalFunction)`.
4. External function was defined as a struct of `{address, selector}`. I changed it to `{selector, address}` to coincide with its encoding form.

There was an idea to get rid of `Type::ExternalFunction` in favor of `Type::Struct(StructDecl::ExternalFunction)` in codegen, however, this would mean boilerplate code for converting types allowed in the AST to types allowed in codegen. In addition, a large refactoring in `cfg.vars` was needed to avoid mismatching types. Thus, this has not been done.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 12:40:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/949" class=".btn">#949</a>
            </td>
            <td>
                <b>
                    Add debug information to LLVM Instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger-labs/solang/issues/584

# Description
- Add debug information to functions and instructions of the LLVM IR generated by `solang`.
- The return instruction `ret` currently does not have the debug location. But it is the case that the return `ret` instruction does not have the corresponding Solidity program statement. It is a special case when it is generated by `solang`.
- Refer to: https://github.com/hyperledger-labs/solang/blob/d05885270708ab822716300f59c6ee1624a5adb3/src/emit/mod.rs#L3404-L3405

# How Has This PR Been Tested?

Please describe the tests that you ran to verify your changes. Please also note any relevant details for your test configuration.

- [x] examples/example.sol
- [x] examples/flipper.sol
- [x] examples/increment.sol
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 02:54:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/947" class=".btn">#947</a>
            </td>
            <td>
                <b>
                    Allow seeds to be passed to external calls for program signing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the seeds parameter to external calls. This does not enable creating PDA style contracts yet, that will come in another PR.

This PR simply adds the seeds to `contract.function{seeds: [ [ seed1 ], [ [ seed2 ]}(arg1, arg2);`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 15:10:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/946" class=".btn">#946</a>
            </td>
            <td>
                <b>
                    Bump solang-parser version for crate publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Foundry would like a new version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 15:03:47 +0000 UTC
    </div>
</div>

