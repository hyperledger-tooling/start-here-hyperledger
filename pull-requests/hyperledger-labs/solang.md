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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/730" class=".btn">#730</a>
            </td>
            <td>
                <b>
                    struct member expressions are not written to graphviz dot file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The handling was incorrect and no nodes were generated.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 13:18:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Refactoring in sema for yul and solidity compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the following refactoring to improve compatibility between Solidity Functions and Yul functions so that we can share the same CFG structures for them both.

1. Parameters are now saved in an `Arc<Vec<Parameter>>>`, because they are shared between `Function`/`YulFunction`, `FunctionsTable` and `ControlFlowGraph`. This way we avoid unnecessary clones from all the elements of a vector.
2. `llvm_symbol` is now under a trait, so that we can implement the same interface for both `Function` and `YulFunction`.
3. Yul Functions are processed in `external_functions`, so that we know which functions should be laid out at each contract.
4. `ty_loc` is now `Option<Loc>` in `Parameter`, because Yul Function parameters might not have a specified type.
5. Yul functions now use `Parameter` instead of `YulFunctionParameter` for saving parameters.
6. The function number in `ControlFlowGraph` is now an enum to distinguish between Yul Functions and Solidity Functions.
7. All Yul functions are centralized in `Namespace`. A Yul function number is its respective index in `Namespace::yul_functions`. Likewise, `FunctionsTable` in `sema/yul/functions.rs` saves such an index and works with an offset for its lookup vector.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 12:24:09 +0000 UTC
    </div>
</div>

