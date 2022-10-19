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
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 16:27:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1038" class=".btn">#1038</a>
            </td>
            <td>
                <b>
                    Encode arguments for constructor call in codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, when we call a constructor, we encode the arguments in emit, using the deprecated EthAbi encoding. A prior step to moving to Borsh is encoding all arguments during codegen. This PR refactors the `Instr::Constructor` to accommodate such changes, alongside the necessary adaptations in emit and codegen.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-13 17:04:39 +0000 UTC
    </div>
</div>

