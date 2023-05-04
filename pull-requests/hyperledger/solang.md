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
                PR <a href="https://github.com/hyperledger/solang/pull/1297" class=".btn">#1297</a>
            </td>
            <td>
                <b>
                    Solve YUL panics for EVM parsing tests
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
                    Casting a pointer to int will truncate the value on 64 bit (e.g. BPF)
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1291" class=".btn">#1291</a>
            </td>
            <td>
                <b>
                    Rework substrate mock runtime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Complete rewrite of the substrate mock runtime:

- Updates to a `wasmi` version with the new API (that's a breaking change requiring some substantial changes anyways)
- Reworked the API of `MockSubstrate` to hide all logic behind functions. This reduces the API surface to a set of functions on a struct, which will make future changes easier.
- Re-implement the host functions so that they resemble up-to-date pallet-contracts more closely
- Introducing separation between Wasm modules (= code), contracts (= code + storage) and accounts (= address +balance + optional contract). This lines the mock implementation up a bit closer to how real nodes work, making implementing additional features in the future easier.

I uncovered a bug in the process. The following contract (adapted from the `calls::try_catch_constructor` test) traps the execution with `MemoryOutOfBounds`:

```
contract c {
    constructor() payable {}

    function test() public returns (int32) {
        int32 x = 0;
        try new other(true) {
            x = 1;
        } catch (bytes memory _c) {
            x = 2;
        }
        return x;
    }
}

contract other {
    constructor(bool rev) public {
        if (rev) {
            revert("foo");
        }
    }

    function _ext() public {}
}
```

This code also fails on a real substrate contracts node (though this returns just `ContractTrapped`, obscuring the underlying reason).. Hence I concluded that the out of bounds memory access most likely stems from a bug in the compiler and disabled the failing test for now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 11:38:50 +0000 UTC
    </div>
</div>

