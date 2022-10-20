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
                PR <a href="https://github.com/hyperledger/solang/pull/1045" class=".btn">#1045</a>
            </td>
            <td>
                <b>
                    Add substrate builtins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a "substrate" file to have custom builtins available, analog to the "solang" file.

Right now there is only the "Hash" type but there will be more in the future. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 08:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1044" class=".btn">#1044</a>
            </td>
            <td>
                <b>
                    Disallow try-catch statements on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Try-catch statements are not supported on Solana. This PR updates the documentation to inform so and adds an error message when someone tries to use such a construct on Solana.

PS: The intention for this PR is to avoid using ABI decoding/encoding for try-catches on Solana, a construction that requires a special case of decoding with a basic block to handle a decoding failure.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 18:34:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1043" class=".btn">#1043</a>
            </td>
            <td>
                <b>
                    Add Solang icon to vscode extension
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure our logo is visible at https://marketplace.visualstudio.com/items?itemName=solang.solang and in vscode itself
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 16:24:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1042" class=".btn">#1042</a>
            </td>
            <td>
                <b>
                    Encode arguments for assert-failure in codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now that all runtime tests for Solana are working with bosh encoding, we can rid Solang of EthAbiEncoding. There is one more instruction that needed refactoring in order to make that a reality. `Instr::AssertFailure` utilizes the old abi encoding scheme implemented in emit (for Solana). This PR refactors the instruction so it encodes its arguments in codegen and allows a future integration with our `trait AbiEncoding`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 11:43:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1041" class=".btn">#1041</a>
            </td>
            <td>
                <b>
                    remove the random builtin function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It is unsafe for most use-cases and will be deprecated in `ink!`. Contract authors should rather use VRF from chain extensions or oracles.

The `seal_random` API is still used to calculate the salt on instantiation (if it is missing). There will be a new API `seal_nonce` which can be used to replace this. I'll do this in another PR once the new nonce API is available in pallets contract.

Side note: In my opinion it is completely safe to remove this built in. It was completely [broken](https://github.com/hyperledger/solang/pull/1025/commits/65018be65d3e95d9a728894e1ac4ee07d4a3aa7a) for IDK exactly how long but no one complained.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 09:59:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1039" class=".btn">#1039</a>
            </td>
            <td>
                <b>
                    Implement more constructor dispatch in cfg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes the following changes:
 - The data account for the solidity contract to be executed must always be the first to be passed
 - Solana deployment code is generated in CFG and not in emit.
 - One test fails without this fix: https://github.com/solana-labs/solana-solidity.js/pull/42
 - Once this is merged I'll release a new version of `@solana/solidity` npm library and re-enable the test

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 16:27:53 +0000 UTC
    </div>
</div>

