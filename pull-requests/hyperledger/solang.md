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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1280" class=".btn">#1280</a>
            </td>
            <td>
                <b>
                    chore(ci): switch to dedicated Solang runners
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
        Created At 2023-04-19 00:01:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1279" class=".btn">#1279</a>
            </td>
            <td>
                <b>
                    Run Ethereum Solidity semantic tests through sema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are many failures. First there are some tests which cause panics in sema. These are explicitly excluded. There are a further 1062 failures. Note the line:

	assert_eq!(errors, 1062);

To see the failures, see:

	cargo test --test evm ethereum_solidity_tests -- --nocapture
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 12:08:56 +0000 UTC
    </div>
</div>

