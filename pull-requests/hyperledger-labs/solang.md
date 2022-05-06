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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/788" class=".btn">#788</a>
            </td>
            <td>
                <b>
                    feat(parser): Gwei unit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Support for `gwei` unit was added in Solidity 0.6.11: https://github.com/ethereum/solidity/blob/develop/Changelog.md#0611-2020-07-07
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 08:37:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/787" class=".btn">#787</a>
            </td>
            <td>
                <b>
                    test(parser): semantic tests from ethereum/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Official Solidity repo contains [semantic tests](https://github.com/ethereum/solidity/tree/develop/test/libsolidity/semanticTests) that we can use to test the support for all languages features i.e. whether Solang can parse any valid Solidity code.

Currently, it breaks tests with such unique errors:
```bash
➜  solang-parser git:(solidity-semantic-tests) cargo test test_solidity_semantic_tests 2>/dev/null | grep -E '^\s+Diagnostic' | awk -F'message: ' '{ print $2 }' | awk -F', notes' '{ print $1 }' | sort -u

"bigint error occurred: invalid digit found in string"
"expected number after decimal point"
"unexpected end of file, expecting \"(\", \"[\", \"abstract\", \"address\", \"bool\", \"byte\", \"bytes\", \"case\", \"constructor\", \"contract\", \"default\", \"enum\", \"error\", \"event\", \"fallback\", \"false\", \"function\", \"import\", \"interface\", \"leave\", \"library\", \"mapping\", \"modifier\", \"payable\", \"pragma\", \"receive\", \"string\", \"struct\", \"switch\", \"this\", \"true\", \"type\", Bytes, DocComment, Int, Uint, address, hexnumber, hexstring, identifier, number, rational, string"
"unrecognised token ')', expected \"++\", \"--\", \".\", \"[\", \"days\", \"ether\", \"finney\", \"gwei\", \"hours\", \"minutes\", \"seconds\", \"szabo\", \"weeks\", \"wei\""
"unrecognised token ')', expected \"address\", \"bool\", \"byte\", \"return\", \"revert\", identifier"
"unrecognised token '.', expected \"(\""
"unrecognised token '.', expected \"(\", \",\", \";\", \"case\", \"constant\", \"default\", \"error\", \"external\", \"internal\", \"leave\", \"override\", \"payable\", \"private\", \"public\", \"pure\", \"return\", \"returns\", \"revert\", \"switch\", \"view\", \"virtual\", \"{\", identifier"
"unrecognised token '.', expected \"for\""
"unrecognised token ';', expected \"(\""
"unrecognised token 'data', expected \"else\""
"unrecognised token 'immutable', expected \"!=\", \"%\", \"%=\", \"&\", \"&&\", \"&=\", \")\", \"*\", \"**\", \"*=\", \"+\", \"++\", \"+=\", \",\", \"-\", \"--\", \"-=\", \".\", \"/\", \"/=\", \":\", \";\", \"<\", \"<<\", \"<<=\", \"<=\", \"=\", \"==\", \"=>\", \">\", \">=\", \">>\", \">>=\", \"?\", \"[\", \"]\", \"^\", \"^=\", \"calldata\", \"case\", \"constant\", \"days\", \"default\", \"error\", \"ether\", \"external\", \"finney\", \"gwei\", \"hours\", \"indexed\", \"internal\", \"leave\", \"memory\", \"minutes\", \"payable\", \"private\", \"public\", \"pure\", \"revert\", \"seconds\", \"storage\", \"switch\", \"szabo\", \"view\", \"weeks\", \"wei\", \"{\", \"|\", \"|=\", \"||\", \"}\", identifier"
"unrecognised token 'return', expected \"else\""
"unrecognised token 'using', expected \"(\", \";\", \"[\", \"abstract\", \"address\", \"bool\", \"byte\", \"bytes\", \"case\", \"contract\", \"default\", \"enum\", \"error\", \"event\", \"false\", \"function\", \"import\", \"interface\", \"leave\", \"library\", \"mapping\", \"payable\", \"pragma\", \"string\", \"struct\", \"switch\", \"this\", \"true\", \"type\", Bytes, DocComment, Int, Uint, address, hexnumber, hexstring, identifier, number, rational, string"
"unrecognised token '{', expected \"!\", \"(\", \")\", \"+\", \"++\", \"-\", \"--\", \"[\", \"address\", \"bool\", \"byte\", \"bytes\", \"case\", \"default\", \"delete\", \"error\", \"false\", \"function\", \"leave\", \"mapping\", \"new\", \"payable\", \"revert\", \"string\", \"switch\", \"this\", \"true\", \"type\", \"~\", Bytes, Int, Uint, address, hexnumber, hexstring, identifier, number, rational, string"
"unrecognised token '{', expected \"case\", \"default\", \"error\", \"leave\", \"revert\", \"switch\", identifier"
```

@seanyoung I guess we can fix these errors at first, and only then merge this PR, so we won't have broken tests in the main branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 05:56:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    Rust 1.59.0 is now required
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solang uses tower-lsp, which depends on dashmap. The latest version of
dashmap requires rust 1.59.0.

dashmap uses `std::thread::available_parallelism()`.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-30 07:45:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    Ensure that virtual functions in abstract contracts can be called
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger-labs/solang/issues/780.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 16:36:34 +0000 UTC
    </div>
</div>

