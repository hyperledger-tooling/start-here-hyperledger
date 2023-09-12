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
                PR <a href="https://github.com/hyperledger/solang/pull/1518" class=".btn">#1518</a>
            </td>
            <td>
                <b>
                    Polkadot: Implemented Node Interactions in Solang's CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This pull request implements `Polkadot` node interactions into `Solang`'s CLI, allowing users to:
- `upload`
- `instantiate`
- `call`
- `remove`  

### Key features include:
- Network Name Parameter: Allows users to specify the Polkadot network by name.

Example: `solang polkadot upload --suri //Alice --network rococo -x --output-json flipper.contract`

### Checklist
- [x] Tested the new commands using a shell script `integration/polkadot/cli_test.sh`.
- [x] Added documentation for the newly implemented commands.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 10:15:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1517" class=".btn">#1517</a>
            </td>
            <td>
                <b>
                    New syntax for contracts on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                Now that we represent contracts by their program id on Solana, we decided to elaborate a new syntax to handle them. Contracts cannot be a type in Solidity, consequently, they cannot be function arguments, function returns nor variables.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 19:40:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1516" class=".btn">#1516</a>
            </td>
            <td>
                <b>
                    Polkadot: Support errors according to `solc`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">polkadot</span>
            </td>
            <td>
                Implement `Panic` and custom errors for the Polkadot target:
- Allow catching `Panic` in sema
- Allow custom errors in sema
- Implement selector  calculation for custom errors
- Refactor try-catch in codegen to allow catch clauses on `Panic` errors in
- Add any custom errors in the metadata
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 08:48:57 +0000 UTC
    </div>
</div>

