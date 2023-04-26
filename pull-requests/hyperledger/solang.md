---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    storage references return values must be set
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solc permits returns values to not have a value assigned, unless its a storage reference. This means that

	function foo() public returns (bool) {}

compiles without warnings, however

	function bar() public returns (string storage) {}

fails with an error diagnostic.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 17:19:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    Solidity keywords were not correctly handled in yul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Many Solidity keywords like `abstract` were incorrectly handled as keywords in yul. 

Cc: @DaniPopes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 16:10:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Use ethereum solidity v0.8.19 testdata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After the testdata directory was moved out of solang-parser, the submodule commit was changed somehow (did not show up in git diff).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 12:28:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1287" class=".btn">#1287</a>
            </td>
            <td>
                <b>
                    Disable default features for lalrpop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `lalrpop` currently has [2 default features](https://docs.rs/crate/lalrpop/latest/features): `lexer`, and `pico-args` for the CLI binary. Neither are being used, and it is recommended to disable default features when the lalrpop lexer is not needed: <https://lalrpop.github.io/lalrpop/quick_start_guide.html>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 22:06:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    [Fix] duplicate code (part 4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related token: #1264
This PR addresses the issue of duplicate code (part 4). I have added a new function `process_event` that helps avoid code duplication.
If this commit is good, I will continue working on resolving the remaining issues in separate commits.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-23 00:01:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1285" class=".btn">#1285</a>
            </td>
            <td>
                <b>
                    The next part of a for loop is an expression, not a statement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should not parse:

	contract C {
	    function f() external {
		for (uint256 i = 0; i < 100; uint256 x = 0) {}
	    }
	}

Fixes https://github.com/hyperledger/solang/issues/1283.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-22 14:31:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1284" class=".btn">#1284</a>
            </td>
            <td>
                <b>
                    Fix new clippy 1.69 lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contains a drive by fix for the build. My guess is that the `ink` umbrella crate doesn't pin it's dependencies, which results in various `ink_* 4.2.0` dependencies being pulled in, despite explicitly pinning `ink = "=4.1.0"` in our `Cargo .toml`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 07:19:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1282" class=".btn">#1282</a>
            </td>
            <td>
                <b>
                    Fixed Duplicate code - 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solving #1262 
Part - 1
I have solved the first using closure and a function. Please give me feedback so that I can finish the other parts. 
Thankyou !
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 11:17:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1281" class=".btn">#1281</a>
            </td>
            <td>
                <b>
                    Do not panic if the value of a constant cannot be evaluated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a constant value makes no sense, then using that constant should not result in any error (previously this paniced).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 09:03:32 +0000 UTC
    </div>
</div>

