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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/956" class=".btn">#956</a>
            </td>
            <td>
                <b>
                    Introduce cli subcommands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fits the CLI more natural.

Now we have:

solang compile --target .. file..
solang language-server --target ..
solang doc --target .. file..

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 13:43:45 +0000 UTC
    </div>
</div>

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

