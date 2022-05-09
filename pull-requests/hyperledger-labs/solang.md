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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/806" class=".btn">#806</a>
            </td>
            <td>
                <b>
                    allow base contracts and libraries to be specified via import object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A contract can be imported via an import object. For example, say you have
a file called a.sol:

	contract A {}
	library L {}

Now, another file can import this via an import object:

	import 'a.sol' as IMP;

	contract C is IMP.A {
		using IMP.L for *;
		constructor() IMP.A() {}
	}

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 10:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    feat(parser): allow `using` on Source Unit level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger-labs/solang/issues/804
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 06:15:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/800" class=".btn">#800</a>
            </td>
            <td>
                <b>
                    Permit immutable on function type contract variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Attributes on contract variables have special handling due to function
types, and function types never had immutable implemented.

Fixes https://github.com/hyperledger-labs/solang/issues/799
Found in https://github.com/hyperledger-labs/solang/pull/787

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 21:11:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    Add keccak hash for addresses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The constant folding pass calculates the Keccak256 hash for number literals, however it was ignoring such calculation for literals of type address. This PR fixes this and solves issue #777.

When this PR is merged, we can also close issue #780 because the contract I posted there builds correctly after this fix.

PS: Contracts for ewasm does not fail after this fix, however the ewasm target still doesn't work, because the emit stage is no implement.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 14:04:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/794" class=".btn">#794</a>
            </td>
            <td>
                <b>
                    infrastructure we need for spl-token and calls to rust contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We need to be able to:
 - Specify the AccountMetas for calls
 - Encode the arguments using a struct
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 14:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/793" class=".btn">#793</a>
            </td>
            <td>
                <b>
                    Add support for functions without parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While working on code generation for Yul statements, I found that the parser did not support yul functions declared without parameters. This PR updates the parser to support this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 13:35:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/792" class=".btn">#792</a>
            </td>
            <td>
                <b>
                    Dead storage incorrect merge of storage load at the same slot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Loading the length of an array and the array itself should not be
merged.

Fixes #776.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 13:16:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/790" class=".btn">#790</a>
            </td>
            <td>
                <b>
                    Remove ambiguity from reaching definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The reaching definition implementation is ambiguous. In statements like `int a, int b = func.call()`, both `a` and `b` have the same definition, because our definition only tracks the block number and the instruction number, leading to errors in optimizations as the one seen in issue #728. 

The eliminate such an ambiguity, I introduced a third dimension in our `Def` structure: the assignment number. This way, in function calls and AbiDecode statements, different variables have different definitions.

This PR fixes issue #728 and improve the reaching definitions implementation from file `reaching_definitions.rs`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 12:48:48 +0000 UTC
    </div>
</div>

