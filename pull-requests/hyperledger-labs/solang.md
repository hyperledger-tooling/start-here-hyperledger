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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/775" class=".btn">#775</a>
            </td>
            <td>
                <b>
                    Only local function pointers should support suffixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Function pointers saved as state variables should no support suffixes "address" and "selector". Only Solidity local variables of type external function pointer support them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 19:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/774" class=".btn">#774</a>
            </td>
            <td>
                <b>
                    solc accepts an 256 bit type as a size argument to new
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We should do the same, but warn about this because it is not efficient
code.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 14:06:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/772" class=".btn">#772</a>
            </td>
            <td>
                <b>
                    Fix associativity of power
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1 ** 2 ** 3 should be parsed like 1 ** (2 ** 3), not (1 ** 2) ** 3.

See https://github.com/foundry-rs/foundry/issues/781#issuecomment-1112109532

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 13:19:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/771" class=".btn">#771</a>
            </td>
            <td>
                <b>
                    Improve compiler diagnostics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure that `now > startTime` gives error about block.timestamp
Improve error for old `function()` syntax
Ensure bad expression errors are surfaced for overloaded function calls

See #744
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 08:19:45 +0000 UTC
    </div>
</div>

