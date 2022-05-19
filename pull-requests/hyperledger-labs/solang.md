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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/836" class=".btn">#836</a>
            </td>
            <td>
                <b>
                    Parse `(new ty){value: 1}(args)`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Three different parse tree for callargs:

	(new D{value: 1})();
	(new D){value: 1}();
	new D{value: 1}();

solc accepts this syntax, so should we.

Fixes https://github.com/hyperledger-labs/solang/issues/818
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 13:13:33 +0000 UTC
    </div>
</div>

