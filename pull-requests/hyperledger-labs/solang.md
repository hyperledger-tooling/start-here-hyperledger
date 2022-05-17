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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/835" class=".btn">#835</a>
            </td>
            <td>
                <b>
                    Fix external call on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes issue #773. The code generation for external function calls from function pointers was not correctly implemented, making Solang panic.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 18:05:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/834" class=".btn">#834</a>
            </td>
            <td>
                <b>
                    Use IdentifierPath instead of Expression in solang-parser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [Using expression provides an unnecessary overhead to matching against fairly simple identifier paths, and this change seeks to simplify that](https://github.com/hyperledger-labs/solang/pull/833)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 16:57:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/832" class=".btn">#832</a>
            </td>
            <td>
                <b>
                    v0.1.11: Nuremberg release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Added
- Added support for Solidity user types
- Support `using` syntax on file scope
- Support binding functions with `using`
- Implemented parsing and semantic analysis of yul (code generation is to
  follow)
- The language server uses the `--import` and `--importmap` arguments
- On Solana, it is possible to set the accounts during CPI using the
  `accounts:` call argument.

### Fixed
- Fixed associativity of the power operator
- A huge amount of fixes improving compatibility with solc

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 15:21:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    uint[1.111111E1111111111111] causes compiler to go into infinite loop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The lexer tries to calculate 10^1111111111111 which will be a very large number. This will take a long time.
    
The lexer should not try to calculate numbers from strings, as this might fail and we do not want the lexer to give up, as no parsing and semantic analysis will be done.

Fixes #829
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 13:43:32 +0000 UTC
    </div>
</div>

