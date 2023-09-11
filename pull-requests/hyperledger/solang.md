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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1514" class=".btn">#1514</a>
            </td>
            <td>
                <b>
                    Add Rename functionality
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature depends on having the right span information for identifiers in the parse tree. Currently, some changes are needed to either add the missing span information in some cases, or improve the already present spans (look for one-off errors). 

The rest of the "goto-*" functions also depend on the availability of proper spans. But in their case, as no modification is made to the source code, lack of accurate spans is less of an issue. But `rename` does modify the source code and hence having incorrect spans can result in unintentionally overwriting pieces of source code, which is highly undesirable. 

The changes made as part of this PR provide the necessary code for `rename` to work. Correcting the parse tree is expected to be done as part of future PRs

A non-exhaustive list of changes to be made to parse tree:  (https://github.com/hyperledger/solang/pull/1411#issuecomment-1648031602)

1. No loc for contract variables type - array_type_dynamic_push.sol L6
2. No loc for constructor base call - abstract_contract_inheritance.sol L14
3. No loc for function modifier arguments - function_modifier_arguments.sol L8
4. No loc for function override base contracts - virtual_functions_override.sol L2
5. Struct literal struct loc and Constructor contract loc not available - inline_assembly.sol L12
6. Internal Function Location wrong when preceded by a contract name. - abi_encode_call.sol L3
7. array with size length function (stored as NumLiteral) - array_type_fixed_length.sol L7
8. struct literals fields point to the struct and not fields, function calls with struct literals => wrong loc - function_arguments.sol L12
9. function calls with contract names : contract defintions absent - - base_contract_function_call.sol L25
10. enum variants vs enum name - struct_type.sol L29
11. using - using.sol L10
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 05:22:33 +0000 UTC
    </div>
</div>

