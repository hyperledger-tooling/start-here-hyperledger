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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/740" class=".btn">#740</a>
            </td>
            <td>
                <b>
                    Calling internal function type broken on solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This has been broken for some time, clearly it was missing a test case.

Fixes issue #733.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 09:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    Shift on integer struct member causes panic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The syntax `self._x >> 112` causes a panic because retrieving the bit
width of a referene to an integer is broken.

Fixes issue #732.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 09:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/738" class=".btn">#738</a>
            </td>
            <td>
                <b>
                    Sema test for casting destructure values is broken
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When the left hand side of a destructure statements is a structure member or array element, the test incorrectly assumed the value was not assignable.
    
Fixes issue #731.
    

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 09:06:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/737" class=".btn">#737</a>
            </td>
            <td>
                <b>
                    Update the development progress in README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm updating our README.md with our latest development progresses. 🥳
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 17:38:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    More info for overload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix https://github.com/hyperledger-labs/solang/issues/707

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 15:22:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/735" class=".btn">#735</a>
            </td>
            <td>
                <b>
                    Update links to discord to the correct channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The links to discord chat is to the discord server, but we can do better
than that and link to the correct channel on the server.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 14:41:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/734" class=".btn">#734</a>
            </td>
            <td>
                <b>
                    chore: typo fixes
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
        Created At 2022-04-12 14:16:58 +0000 UTC
    </div>
</div>

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

