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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/761" class=".btn">#761</a>
            </td>
            <td>
                <b>
                    WIP: Add spl-token integration
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
        Created At 2022-04-22 13:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/760" class=".btn">#760</a>
            </td>
            <td>
                <b>
                    Do not allow yul suffixes on certain variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While working with YUL code generation, I found out that we were not detecting if the usage of suffixes was correct for Solidity local variables. This PR fixes this bug that I found.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 14:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/759" class=".btn">#759</a>
            </td>
            <td>
                <b>
                    Fix assigning to array subscript when array element is array
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dereferencing an array did not make the array writable.

Fixes issue found here:

https://stackoverflow.com/questions/71789212/solang-panicked-at-type-not-allowed

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 11:00:55 +0000 UTC
    </div>
</div>

