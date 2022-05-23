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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    Do not raise warning for function parameters saved in storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a minor issue I found while working on issue #813.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 17:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    Refactor Solang docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR splits the old `language.rst` file into multiple files so that the user can see the sections on the navigation bar. I also re-organized the order of items in the bar.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 14:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/843" class=".btn">#843</a>
            </td>
            <td>
                <b>
                    Allow types to be called error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solc allows this too.

Found in https://github.com/hyperledger-labs/solang/pull/787

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-21 07:45:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    Fix parse location of FunctionCallBlock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Expression::FunctionCallBlock` location does not surround entire
expression, and this fixes that by moving the location start to the
beggining of the expression. This also adds `pretty_assertions`
for easier debugging of dot files in tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 09:53:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/841" class=".btn">#841</a>
            </td>
            <td>
                <b>
                    Parse assembly statement flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just update the parser and produce errors, no actual support yet.

See https://github.com/hyperledger-labs/solang/issues/828 and #787 

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 09:35:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/840" class=".btn">#840</a>
            </td>
            <td>
                <b>
                    Parse override(list) syntax on variable definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - The parser does not parse an override list specified on a variable definition
- The override list may be specified via an import path.

Found in #787 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 09:06:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/839" class=".btn">#839</a>
            </td>
            <td>
                <b>
                    Fix parser locations of expressions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The parser locations for unary and binary expression are inconsistent.
Often only the operator itself is included, and not operand(s). This is
causes incorrect diagnostics.
```
/home/sean/git/solang/tests/contract_testcases/substrate/arrays/array_dimensions.sol:3:21-22: error: zero size array not permitted
Line 3:
	bool[10 - 10] x;
	--------^
```
This is now fixed:
```
error: zero size array not permitted
  ┌─ /home/sean/git/solang/tests/contract_testcases/substrate/arrays/array_dimensions.sol:3:18
  │
3 │             bool[10 - 10] x;
  │                  ^^^^^^^
```
This issue was found by the Foundry work to create a formatter based on
the solang-parser, see https://discord.com/channels/900503503162724452/975868842125455390/976527889166135357

---

This also means we have to deal with overlapping expressions in the language server
    
Now the locations for binary expressions overlaps with their operands. This means that we have overlapping locations for hovers in the language server. We deal with this by finding all matching hovers, and returning the hover which is the shortest.
    
Unfortunately this involves a linear scan of the hovers. This is linear scan of memory, so it should be fast. However, there may be a better data structure we can choose for this, should performance be an issue.

I was thinking we could use something like an r* tree but this is a bit heavy for our use-case. Any suggestions?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 08:54:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    Load stdlib only once
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes #807. We are now only loading the stdlib module only once and linking it against any other modules we create. Although LLVM types are global, I believe LLVM adds a `.0` to the end of the type name for disambiguation, because it does not check if two types of equal names represent the same structure in the memory. In this sense, whenever we load stdlib again, LLVM understands that is a totally new module and tries to disambiguate type names.

Please, @seanyoung check if I did not remove any necessary pointer cast.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 14:31:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/837" class=".btn">#837</a>
            </td>
            <td>
                <b>
                    Refactor emit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In order to solve #807, I need to implement changes in Binary. This PR removes Binary from `emit/mod.rs`, so that I can work on it without modifying the `TargetRuntime`.

The issue of LLVM renaming our types happens because we load the stdlib multiple times. Instead, we must load it once, build an LLVM module and link this same module to all other ones we create. Once this PR is merged, I'll submit my changes.

In addition, I split the contract test into three functions, so that they run in parallel and make our testing faster. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 12:41:32 +0000 UTC
    </div>
</div>

