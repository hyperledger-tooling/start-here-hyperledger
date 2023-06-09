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
                PR <a href="https://github.com/hyperledger/solang/pull/1360" class=".btn">#1360</a>
            </td>
            <td>
                <b>
                    WIP tornado cash on Substrate  :rocket: 
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
        Created At 2023-06-07 18:44:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1359" class=".btn">#1359</a>
            </td>
            <td>
                <b>
                    fix(refactor): Fix duplicate code for issue #1265
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to solve the duplicate code issue in #1265 .

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 13:15:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1358" class=".btn">#1358</a>
            </td>
            <td>
                <b>
                    Substrate: Add an integration test for chain extensions
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
        Created At 2023-06-06 20:19:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1357" class=".btn">#1357</a>
            </td>
            <td>
                <b>
                    Use custom substrate CI image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use [a custom node](https://github.com/hyperledger/solang-substrate-ci) for the integration tests. This tests contains chain extension which I'll add integration tests for in a followup PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 17:51:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1356" class=".btn">#1356</a>
            </td>
            <td>
                <b>
                    Improve unused variable elimination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following code causes an invalid memory access:

```solidity
function foo() public pure returns (bytes memory) {
    bytes b1 = hex"41";
    bytes b2 = hex"42";
 
   b2.push(0x41);
   return b1;
}

```

That happens because the unused variable elimination removes the declaration `bytes b2`, but maintains the `push`. This PR improves the elimination algorithms so much so that it removes the unnecessary pushes and pops if there is no actual read to the array in the function. It also takes care not to discard such operations when arrays are pointers to either storage or memory.

In addition, the error message for unused function parameter has been updated to `function parameter 'my_parameter' is unused`. When the parameter is a vector and has a push but no read, writing that it is `never read` is not the proper warning.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 21:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1355" class=".btn">#1355</a>
            </td>
            <td>
                <b>
                    Fix Anchor integration test
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
        Created At 2023-06-05 14:04:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1353" class=".btn">#1353</a>
            </td>
            <td>
                <b>
                    Do not pin `ink!` dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was required for 4.1.0 because back then we were on rust 1.65 while 4.2.0 was on 1.68

Fixes #1351 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-04 08:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1352" class=".btn">#1352</a>
            </td>
            <td>
                <b>
                    fix(docs): Minor typo fixes for installation documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to fix minor typos in the installation documentation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-03 10:07:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1350" class=".btn">#1350</a>
            </td>
            <td>
                <b>
                    Do not allow push and pop in fixed length arrays
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We presently allow pushed and pops from fixed length arrays, leading to a panic in emit. This PR disallows such operations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 19:14:56 +0000 UTC
    </div>
</div>

