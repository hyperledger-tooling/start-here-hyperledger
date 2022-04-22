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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/752" class=".btn">#752</a>
            </td>
            <td>
                <b>
                    Implement codegen for yul primitive expressions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the code generation for YUL primitive expressions. I also provided unity tests for the function I created.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 17:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/751" class=".btn">#751</a>
            </td>
            <td>
                <b>
                    Fix interface inheritance bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a bug, in which we couldn't not call a function from an interfaced that was inherited from another one.

This is one of the bugs found in issue #744.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-19 15:29:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/749" class=".btn">#749</a>
            </td>
            <td>
                <b>
                    Create codegen::Builtin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates a `codegen::Builtin` so that we can have a single interface to manage both Yul and Solidity Builtins, some of which are common.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 18:25:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/748" class=".btn">#748</a>
            </td>
            <td>
                <b>
                    Implement type definition syntax
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ethereum Solidity introduces a new syntax for user defined types, see:

https://docs.soliditylang.org/en/v0.8.13/types.html

Documentation for the syntax is in the documentation of this commit, and not repeated here.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-17 09:26:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/747" class=".btn">#747</a>
            </td>
            <td>
                <b>
                    feat(parser): user defined value types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger-labs/solang/issues/746

Better suggestions on resolving ambiguity with `type()` builtin are welcome 😄 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 21:58:29 +0000 UTC
    </div>
</div>

