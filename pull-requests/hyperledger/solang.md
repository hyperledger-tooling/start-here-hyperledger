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
                PR <a href="https://github.com/hyperledger/solang/pull/1301" class=".btn">#1301</a>
            </td>
            <td>
                <b>
                    update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates some dependencies.

Most notably inkwell 0.2.0 which now supports LLVM 16 :eyes: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 13:49:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1300" class=".btn">#1300</a>
            </td>
            <td>
                <b>
                    Update substrate-contracts-node to v0.25.0
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
        Created At 2023-05-08 09:59:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1299" class=".btn">#1299</a>
            </td>
            <td>
                <b>
                    Enable tests for stdlib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces the following changes:
1. Stdlib is now build directly with `cargo build`, so all the wasm and bpf files have been removed from the repository.
2. Enable the tests for the stdlib. If nothing fails within two minutes, the test passes.
3. Enable the linter `clang-format` for the stdlib. All C files have been reformatted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 21:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1298" class=".btn">#1298</a>
            </td>
            <td>
                <b>
                    Do not panic if variable accessor function has duplicate argument names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This can only arise with nested mapping:

```solidity
contract test {
    mapping(uint nameSame => mapping(uint name1 => mapping(uint nameSame => uint 
name3) name6) name4) public name5;
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 08:31:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1297" class=".btn">#1297</a>
            </td>
            <td>
                <b>
                    Solve YUL panics for EVM semantic tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I fixed a problem in which we were trying to fetch a function header that was not added to the set of processed headers, because there was an error in processing it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 21:24:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1296" class=".btn">#1296</a>
            </td>
            <td>
                <b>
                    fixed the duplicate code by adding functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed duplicate code by replacing it using functions, kindly guide me if I am on right direction or not.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 13:26:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1295" class=".btn">#1295</a>
            </td>
            <td>
                <b>
                    Compare the full 64 bits address on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                vector_new() takes an initializer arguments, which has as special value
for "no initializer". We should check the full 64 bits, rather than
casting the lower 32 bits to int.

This change exposes a bug in the old BPF target in Solana's LLVM fork. Switching 
to the newer SBF target fixes the issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 10:43:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1294" class=".btn">#1294</a>
            </td>
            <td>
                <b>
                    Update ink! caller integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the caller contract to use the latest ink! release. I also re-structured the solidity code to try and make what's going on in there obvious. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 14:25:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1293" class=".btn">#1293</a>
            </td>
            <td>
                <b>
                    Fix build with lalrpop 0.19.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 0.19.12 version of the lalrpop crate broke the build.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 09:02:58 +0000 UTC
    </div>
</div>

