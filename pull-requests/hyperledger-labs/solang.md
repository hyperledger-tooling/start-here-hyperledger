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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/757" class=".btn">#757</a>
            </td>
            <td>
                <b>
                    Fix standalone function call bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a bug found in issue #744. We found out that when a function that returns multiple values was invoke as a top level statement, the compiler emitted an error. In sum, the following constructions should be allowed:

```solidity
function multipleReturns() returns (int, int) {
    return (1, 2)
}

function test() returns int {
    multipleReturns();
    return 3;
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 17:03:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/756" class=".btn">#756</a>
            </td>
            <td>
                <b>
                    @return doccomments on unnamed returns permitted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This doc comment is not permitted:
```
// @return feh
// @return foo
function f3() pure returns (int, int) { return (1, 2); }
```
Allow unnamed returned value to have doc comments, while ensuring that
there is on per return.

Also fix the location of doc-comments in diagnostics.

Found:
https://stackoverflow.com/questions/71789212/solang-panicked-at-type-not-allowed

The issue described on stackoverflow is not fixed yet.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 12:32:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/753" class=".btn">#753</a>
            </td>
            <td>
                <b>
                    Call struct member address does not work
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 Call struct member address does not work
    
The address is not loaded.
    
Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 08:46:44 +0000 UTC
    </div>
</div>

