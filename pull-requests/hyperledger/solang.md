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
                PR <a href="https://github.com/hyperledger/solang/pull/1527" class=".btn">#1527</a>
            </td>
            <td>
                <b>
                    Fix type(int256).min in comparisons
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When resolving comparisons, we don't know what the types of the operands are so we resolve with `ResolveTo::Unknown`. In this path, there is an mistake in the bounds check for negative integers.

Fixes https://github.com/hyperledger/solang/issues/1523
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 12:00:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1522" class=".btn">#1522</a>
            </td>
            <td>
                <b>
                    Fix recursive struct issue
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
        Created At 2023-09-13 22:32:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    Verify magic number in fallback
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, we do not check the magic number when we enter a fallback function. If it modifies or read the data account, a malefactor can forge an account so that the function would read or write malicious data. This PR fixes such an issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-12 19:59:04 +0000 UTC
    </div>
</div>

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

