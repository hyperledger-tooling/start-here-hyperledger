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
                PR <a href="https://github.com/hyperledger/solang/pull/1552" class=".btn">#1552</a>
            </td>
            <td>
                <b>
                    Bugfix: Variables declared in return param can have a storage location
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Variables declared as return parameters can have a storage location too.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 07:57:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1551" class=".btn">#1551</a>
            </td>
            <td>
                <b>
                    Purge the compiler of `codegen::Expression::List`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The expression was unused.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 20:59:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1549" class=".btn">#1549</a>
            </td>
            <td>
                <b>
                    Support `address.code` in sema
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
        Created At 2023-09-22 15:25:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1548" class=".btn">#1548</a>
            </td>
            <td>
                <b>
                    Add code coverage bot 🤖
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Coverage reports will be stored [here](https://app.codecov.io/gh/hyperledger/solang).

According to Codecov's documentation,
> Once merged to the default branch, subsequent pull requests will have checks and report comment.

This is an example of how comments look like: https://github.com/solana-labs/solana/pull/33363#issuecomment-1730528544
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 14:53:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1547" class=".btn">#1547</a>
            </td>
            <td>
                <b>
                    Allow seeds to be passed into functions as string[] or string[][]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                This fixes this Solidity and similar constructs.

```solidity
import "solana-library/spl_token.sol";

contract c {

    // Invoke the token program to mint tokens to a token account, using a PDA as the mint authority
    function mintTo(address mint, address account, address authority, uint64 amount, bytes[] seeds) internal {
        // Prepare instruction data
        bytes instructionData = new bytes(9);
        instructionData[0] = uint8(7); // MintTo instruction index
        instructionData.writeUint64LE(amount, 1); // Amount to mint

        // Prepare accounts required by instruction
        AccountMeta[3] metas = [
            AccountMeta({pubkey: mint, is_writable: true, is_signer: false}),
            AccountMeta({pubkey: account, is_writable: true, is_signer: false}),
            AccountMeta({pubkey: authority, is_writable: true, is_signer: true})
        ];

        // Invoke the token program with prepared accounts and instruction data
        SplToken.tokenProgramId.call{accounts: metas, seeds: seeds}(instructionData);
    }
}
```

Fixes https://github.com/hyperledger/solang/issues/1433
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 08:40:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1546" class=".btn">#1546</a>
            </td>
            <td>
                <b>
                    Update and fix target config file templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We don't want to maintain the same file twice. One version was outdated. The other one contained an invalid config for  `wasm-opt`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-20 15:12:00 +0000 UTC
    </div>
</div>

