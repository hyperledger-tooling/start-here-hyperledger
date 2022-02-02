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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    The parser should record all comments
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
        Created At 2022-02-02 11:10:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    Permit assigment in ternary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Support the following construct:

    function minimum(uint64 x, uint64 y) public pure returns (uint64 z) {
        x >= y ? z = y : z = x;
    }

Fixes #654 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 15:12:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    Permit assembly keywords in solidity and vice versa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This ensures that `switch`, `default`, `case`, and `leave` are permitted in solidity, and that `return` is permitted in assembly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 09:41:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    Allow comparisons between bytes32 and 0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The constant 0 can be implicitly converted to a fixed-bytes value, so
the following statement should be allowed:

function foo(bytes4 bs) public returns (bool) {
	return bs > 0;
}

Found in the example code of #643

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 17:25:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    Permit larger type to be used as a value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                value or balance is uint128 on ewasm and substrate, and uint64 on
solana. Lots of existing solidity code uses uint256, so permit this but
insert checks and warn about it.

Fixes #632 
Replaces #637 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 13:44:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    Fix invalid llvm IR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                LLVM permits invalid IR in many cases, which llc or llvm-dis does not permit.

Fixes #641 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 10:05:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/648" class=".btn">#648</a>
            </td>
            <td>
                <b>
                    Ensure that address struct members can be saved to state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #642
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 17:06:13 +0000 UTC
    </div>
</div>

