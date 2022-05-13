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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    Don't run the linux-arm64 tests on PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These tests are run on a single traverse ten64, and this takes 38
minutes. This is too long is holding up PR merges and test completion.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 18:15:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    Do not load from storage when reference is needed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes #789. We were loading a value from storage whenever we encountered a storage reference. However, we should not load if we want the reference, not the value.

To solve this, modified `fn destructure_load` and renamed it to `fn cast_and_try_load`. Another option would be merging such a function with `codegen::Expression::cast`, however I am not sure if the cast function should be allowed to manage the CFG.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 17:01:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    WIP: Partial support for Yul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables partial support for Yul in code generation. Tests are still missing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 13:29:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    Permit negative components in scientific notation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                200e-2 is a NumberLiteral (2)
2e-2 is a RationalNumber(0.02)

Fixes #819
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 11:52:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/822" class=".btn">#822</a>
            </td>
            <td>
                <b>
                    Ensure that method on number literal works correctly.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure that `42.double()` works with using.
```
function double(int x) pure returns (int) { return x * 2; }

using {double} for int;

contract C {
	function foo() pure public returns (int) {
		return 42.double();
	}
}
```
Fixes https://github.com/hyperledger-labs/solang/issues/820
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 09:08:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/817" class=".btn">#817</a>
            </td>
            <td>
                <b>
                    body of for loop may be if without else
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This particular syntax was not parsed:

	for (;;) if (false) return 0;

Fixes https://github.com/hyperledger-labs/solang/issues/798

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 14:27:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    Parse revert statements with named arguments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                	revert Foo({bar: 1});

These can only be used with custom errors, which are not supported yet.
However, amend the parser so that we can give a nicer error message.

Found in #787 

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 13:13:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/815" class=".btn">#815</a>
            </td>
            <td>
                <b>
                    doccomment are allowed anywhere
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                	contract c {}
	/// foo

The comment foo is not attached to anything.

This fixes https://github.com/hyperledger-labs/solang/issues/812

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 11:40:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/814" class=".btn">#814</a>
            </td>
            <td>
                <b>
                    Permit function list in using syntax
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is new syntax introduced with solc 0.8.13.

	function foo(int) {};
	function foo2(int) {};

	contract c {
		using {foo,foo2} for int;

		function test(int c) public {
			c.foo();
			c.foo2();
		}
	}

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-07 19:04:24 +0000 UTC
    </div>
</div>

