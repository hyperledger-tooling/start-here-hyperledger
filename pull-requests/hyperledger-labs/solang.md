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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/959" class=".btn">#959</a>
            </td>
            <td>
                <b>
                    Make --generate-debug-info hidden
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature is incomplete and does not have any users yet. For example, there is a debugging endpoint for Solana in the works, but this is not finished yet. Also, this will be useful for static analysis, which requires debug information for higher-level type information.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 08:39:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/958" class=".btn">#958</a>
            </td>
            <td>
                <b>
                    Update roadmap for Substrate target
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @athei we are reworking the solang roadmap. I mapped  the milestones from the solang Bounty Proposal into the roadmap as follows:
- V0.2: Includes Milestones 1, 2, 3, 4, 6
- V0.3: Includes Milestones 5, 7, 8, 9
- V0.4: Includes Milestones 10, 11

Of course nothing will be set in stone here. What do you think?

Signed-off-by: Cyrill Leutwiler <bigcyrill@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 20:40:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/957" class=".btn">#957</a>
            </td>
            <td>
                <b>
                    Bytes of Type::Bytes must be reversed before encoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Type::Bytes` is represented as an integer in LLVM. This means its bytes are reversed if we use the `Instr::WriteBuffer` instruction. This PR fixes this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 18:49:06 +0000 UTC
    </div>
</div>

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

