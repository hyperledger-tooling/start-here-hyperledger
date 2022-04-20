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

// @return feh
// @return foo
function f3() pure returns (int, int) { return (1, 2); }

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/745" class=".btn">#745</a>
            </td>
            <td>
                <b>
                    Fix lexing of /**/
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This type of comment was not recognised by the lexer.

See #744.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 09:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/743" class=".btn">#743</a>
            </td>
            <td>
                <b>
                    feat: support projections in revert statement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I tried to fix this but I believe Hit some lalrpop issues, so this won't build I'm afraid. 
But not sure what the proper fix for this would be, so I'd need some help


Background

this is a valid revert:

```solidity
        function doRevert2() internal pure {
             revert LibName.ErrorName();
        }
```

if an error is defined inside a library `LibName` 

the solidity grammar states the revert stmt is `"revert" + expr + call-arg-list`
But I think only this is valid (Id)? ("." Id)*
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 17:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/742" class=".btn">#742</a>
            </td>
            <td>
                <b>
                    feat: support byte as yulidentifier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                prior to this `byte` was tokenized as `Token::Bytes(1)` as prior to 0.8.0 `byte` used to be an alias for `bytes1`

however this breaks the assembly `byte` function

```solidity
            assembly {
                v := byte(0, mload(add(signature, 0x60)))
            }
```

This PR

* adds a `"bytes" => Byte` token, that will be `Bytes(1)` if used as type or a yulidentifier

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 16:58:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/741" class=".btn">#741</a>
            </td>
            <td>
                <b>
                    Create codegen::Expression and refactor codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR refactor code generation. The main addition was the `codegen::Expression`. This means we no longer depend on `ast::Expression` to build the CFG. I've managed to improve some other stuff:

1. Now, we have a `cast` function for codegen. 
2. Sema's `cast` function is now a method of `ast::Expression`.
3. I created traits for common functions to facilitate implementing methods with generic arguments.
4. I removed from the AST expressions that do not belong there, except `FunctionArg`, to which I couldn't find an easy solution.
5. Some AST expressions do not exist is the CFG, so I removed references to them in codegen.
6. As we are branching at every AND and OR expression, they do not exist in `codegen::Expression`. However, I left some block comments containing the code to handle those cases, in case we add them in nearby future.

PS: This PR modifies 56 files, so please, @seanyoung, be pedantic!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 14:53:55 +0000 UTC
    </div>
</div>

