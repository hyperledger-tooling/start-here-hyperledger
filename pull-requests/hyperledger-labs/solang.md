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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    Move to clap 3.0
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
        Created At 2022-01-04 16:08:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    Provide method for accessing accounts on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates a builtin array `tx.accounts[]` which gives access to the tx accounts, so it is possible to do things like:

```
     AccountInfo ai = tx.accounts[0];
     ai.lamports += 1;
     uint64 total_supply = tx.accounts[1].data.readUint64LE(4);
```
    
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 11:46:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #617 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-31 11:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Make solidity parser a standalone crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is essentially a followup on #597 and makes the solidity parser a standalone crate (`solang-parser`)

## Changes
* move `src/parser/*` to `solang-parser`, including lalrpop build
* move `src/sema/ast/Diagnostic` related structs to `solang-parser/src/diagnostics/`. This was necessary because the parser's error is the Diagnostic, but has the downside that some `Diagnostic` implementation is now in two places:
  * made `src/sema/ast/Diagnostic::formatted_message` a function that accepts a `&Diagnostic` instead
* rm unused dependencies in solang 
* reexport the parser, so it doesn't break
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 19:45:59 +0000 UTC
    </div>
</div>

