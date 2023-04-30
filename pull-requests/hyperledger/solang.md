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
                PR <a href="https://github.com/hyperledger/solang/pull/1291" class=".btn">#1291</a>
            </td>
            <td>
                <b>
                    Rework substrate mock runtime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Complete rewrite of the substrate mock runtime:

- Updates to a `wasmi` version with the new API (that's a breaking change requiring some substantial changes anyways)
- Reworked the API of `MockSubstrate` to hide all logic behind functions. This reduces the API surface to a set of functions on a struct, which will make future changes easier.
- Re-implement the host functions so that they resemble up-to-date pallet-contracts more closely
- Introducing separation between Wasm modules (= code), contracts (= code + storage) and accounts (= address +balance + optional contract). This lines the mock implementation up a bit closer to how real nodes work, making implementing additional features in the future easier.

I uncovered a bug in the process. The following contract (adapted from the `calls::try_catch_constructor` test) traps the execution with `MemoryOutOfBounds`:

```
contract c {
    constructor() payable {}

    function test() public returns (int32) {
        int32 x = 0;
        try new other(true) {
            x = 1;
        } catch (bytes memory _c) {
            x = 2;
        }
        return x;
    }
}

contract other {
    constructor(bool rev) public {
        if (rev) {
            revert("foo");
        }
    }

    function _ext() public {}
}
```

This code also fails on a real substrate contracts node (though this returns just `ContractTrapped`, obscuring the underlying reason).. Hence I concluded that the out of bounds memory access most likely stems from a bug in the compiler and disabled the failing test for now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 11:38:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    storage references return values must be set
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solc permits returns values to not have a value assigned, unless its a storage reference. This means that

	function foo() public returns (bool) {}

compiles without warnings, however

	function bar() public returns (string storage) {}

fails with an error diagnostic.

This PR also changes the `contract_testcases`. The expected diagnostics are listed in the source file, in the same way as this is done for solc tests. This makes the `contract_testcases` much more useful. 

I am wondering if there is much justification for keeping the .dot files in the repo any more. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 17:19:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    Solidity keywords were not correctly handled in yul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Many Solidity keywords like `abstract` were incorrectly handled as keywords in yul. 

Cc: @DaniPopes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 16:10:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Use ethereum solidity v0.8.19 testdata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After the testdata directory was moved out of solang-parser, the submodule commit was changed somehow (did not show up in git diff).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 12:28:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1287" class=".btn">#1287</a>
            </td>
            <td>
                <b>
                    Disable default features for lalrpop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `lalrpop` currently has [2 default features](https://docs.rs/crate/lalrpop/latest/features): `lexer`, and `pico-args` for the CLI binary. Neither are being used, and it is recommended to disable default features when the lalrpop lexer is not needed: <https://lalrpop.github.io/lalrpop/quick_start_guide.html>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 22:06:49 +0000 UTC
    </div>
</div>

