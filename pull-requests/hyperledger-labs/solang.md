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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    Rust 1.59.0 is now required
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solang uses tower-lsp, which depends on dashmap. The latest version of
dashmap requires rust 1.59.0.

dashmap uses `std::thread::available_parallelism()`.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-30 07:45:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    Ensure that virtual functions in abstract contracts can be called
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger-labs/solang/issues/780.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 16:36:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/775" class=".btn">#775</a>
            </td>
            <td>
                <b>
                    Only local function pointers should support suffixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Function pointers saved as state variables should no support suffixes "address" and "selector". Only Solidity local variables of type external function pointer support them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 19:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/774" class=".btn">#774</a>
            </td>
            <td>
                <b>
                    solc accepts an 256 bit type as a size argument to new
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We should do the same, but warn about this because it is not efficient
code.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 14:06:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/772" class=".btn">#772</a>
            </td>
            <td>
                <b>
                    Fix associativity of power
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1 ** 2 ** 3 should be parsed like 1 ** (2 ** 3), not (1 ** 2) ** 3.

See https://github.com/foundry-rs/foundry/issues/781#issuecomment-1112109532

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 13:19:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/771" class=".btn">#771</a>
            </td>
            <td>
                <b>
                    Improve compiler diagnostics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure that `now > startTime` gives error about block.timestamp
Improve error for old `function()` syntax
Ensure bad expression errors are surfaced for overloaded function calls

See #744
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 08:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/770" class=".btn">#770</a>
            </td>
            <td>
                <b>
                    Consistent use of single quotes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
    We have ‘x’, `x`, and ‘x‘. Always use 'x'.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 12:11:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/769" class=".btn">#769</a>
            </td>
            <td>
                <b>
                    Give a nice error message when 'now' is used
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
        Created At 2022-04-27 11:43:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/767" class=".btn">#767</a>
            </td>
            <td>
                <b>
                    Fix require() not found and staticcall in view function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                More fixes for #744. 

Two commits:

address.call() is permitted in view functions on ewasm and solana

and:

Error of garbage argument to builtin function not surfaced
   
A function call like:
    
            require("a" > 2);
    
Will just give the diagnostic:
    
             error: cannot find overloaded function which matches signature

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 09:01:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    Refactor diagnostics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR refactors the diagnostics vectors inside `Namespace`. Now, we have a data structure to handle diagnostics. It helps us keep track of the quantity of warnings and errors we have, without needing to traverse the entire vector. We should only manage the `Vec<Diagnostic>` using the `struct Diagnostics` because we keep track of the existence of errors in the vector. This way, all attributes of the aforementioned struct are private.

In addition, we only emit warnings for unused variables and events if there is no error in the contract. This avoids false positives.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 17:23:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/765" class=".btn">#765</a>
            </td>
            <td>
                <b>
                    Yul suffixes for call data arrays should consider the last dimension
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a bug I found while working on the the code generation for Yul. The suffixes for call data dynamic arrays should consider the array's last dimension only.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 12:47:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/764" class=".btn">#764</a>
            </td>
            <td>
                <b>
                    Delay resolving on contract variable initializers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The initializer to contract variable may only be done once all the base
contract functions are resolved, as the initializer might be reference to
a function in base contract, for example:

    contract b {
        function testPtr(int a) public pure returns (int) {
            return a/2;
        }
    }

    contract testing is b {
        function(int) external pure returns (int) sfPtr = this.testPtr;
    }

Note this also fixes code like:

    contract test {
        uint x = y + 102;
        uint y = 102;
    }

Fixes #762

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 11:09:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/763" class=".btn">#763</a>
            </td>
            <td>
                <b>
                    Remove Expression::FunctionArg from ast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This expression type does not belong in the ast. It is used in the
implicit accessor functions of public storage variables. Rather than
using a codegen-like expression, create a proper symbol table entries
for the arguments and retrieve them.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 16:24:30 +0000 UTC
    </div>
</div>

