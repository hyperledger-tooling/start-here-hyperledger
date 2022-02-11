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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/663" class=".btn">#663</a>
            </td>
            <td>
                <b>
                    Bump dependencies
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
        Created At 2022-02-11 09:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/662" class=".btn">#662</a>
            </td>
            <td>
                <b>
                    feat(parser): add support for custom error types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add
* ErrorDefinition
* ErrorParameter

support in lalrpop and ast types (based on existing EventDef/EventParam), following https://docs.soliditylang.org/en/v0.8.11/grammar.html#a4.SolidityParser.errorDefinition


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 17:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/661" class=".btn">#661</a>
            </td>
            <td>
                <b>
                    Fix line comments that end in non-ascii character
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The lexer assumed the last character was 1 byte.

Fixes #660 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 10:25:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/659" class=".btn">#659</a>
            </td>
            <td>
                <b>
                    Implement solana AccountMeta builtin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should make it possible to use spl-token
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 15:12:46 +0000 UTC
    </div>
</div>

