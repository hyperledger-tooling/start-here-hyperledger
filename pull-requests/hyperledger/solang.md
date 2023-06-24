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
                PR <a href="https://github.com/hyperledger/solang/pull/1386" class=".btn">#1386</a>
            </td>
            <td>
                <b>
                    Do not inline `vector_new`
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
        Created At 2023-06-23 18:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1384" class=".btn">#1384</a>
            </td>
            <td>
                <b>
                    Access payer account using `tx.accounts.account_name`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates the infrastructure for accessing accounts with `tx.accounts.account_name`. Presently, we can only access accounts declared with the `@payer` annotation, but our goal is to make this possible for all accounts declared with annotations (this is not implemented yet). 

The documentation I wrote is very terse, because my plan is to add more details when I have the `@reader`, `@mutable`, `@signer` and `@mutableSigner` implemented.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 14:50:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1383" class=".btn">#1383</a>
            </td>
            <td>
                <b>
                    Update roadmap on README
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
        Created At 2023-06-23 08:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1381" class=".btn">#1381</a>
            </td>
            <td>
                <b>
                    Followup regarding subxt test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Do not rely on a CI node to be able to compile the tests
* Compile the tests in parallel
* Add a short README  hinting about how to maintain this
* Set me as the codeowner

@extraymond if you see this and wondering why providing the metadata directly (again) instead of fetching from the node. I did not think about that if we fetch it directly, anyone clonening the Solang repo will also have to have our CI node running, otherwise compilation fails. This is a bit awkward so we decided to change it again.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 20:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1380" class=".btn">#1380</a>
            </td>
            <td>
                <b>
                    Fix a bunch of subxt-tests rust warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If you don't have a substrate node running you still get errors. I don't know what to do about that.

I've tried putting it in `#[cfg(test)]` which didn't help.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 14:53:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1378" class=".btn">#1378</a>
            </td>
            <td>
                <b>
                    Wasm linker: Do not strip off empty data sections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR gets rid of the wasm-opt complaining about `warning: data index out of bounds in name section, data subsection: .bss at index 0`.


This was caused by us just skipping these sections. By doing so, the resulting Wasm blob size will be smaller without (it's just uninitialized data):

```
 - segment[10] <.bss.selector> memory=0 size=4 - init i32=608
  - 0000260: 0000 0000                                ....
 - segment[11] <.bss.calldata_len> memory=0 size=4 - init i32=612
  - 0000264: 0000 0000                                ....
 - segment[12] <.bss.scratch_len> memory=0 size=4 - init i32=616
  - 0000268: 0000 0000                                ....
 - segment[13] <.bss.scratch> memory=0 size=32768 - init i32=624
  - 0000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
  - ...
```

However, `wasm-opt` will do the same, so we can just rely on `wasm-opt` to do it correctly. I additionally checked the Wasm blob size of various contracts (with `wasm-opt` enabled) and the code sizes stay exactly the same after this change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 08:15:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1377" class=".btn">#1377</a>
            </td>
            <td>
                <b>
                    Avoid repeated global strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When debugging the issue #1367, I found out that we keep emitting repeated global strings. The LLVM IR for the contract pointed in such an issue had the string `math overflow,\0A` defined 1008 times.

This PR DOES NOT solve #1367, but it is something that needed a fix.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 21:13:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1376" class=".btn">#1376</a>
            </td>
            <td>
                <b>
                    Substrate: Implement call flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Substrate knows [flags](https://github.com/paritytech/substrate/blob/6e0059a416a5768e58765a49b33c21920c0b0eb9/frame/contracts/src/wasm/runtime.rs#LL392C27-L392C27) for contract calls. Until now we just always set them to 0. However we'll need them for more ergonomic `delegatecall` support and giving contract authors manual control over contract reentrancy. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 19:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1374" class=".btn">#1374</a>
            </td>
            <td>
                <b>
                    Implicit accessor function should return struct members, not struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the acessor function returns a single struct, then the members should be returned. If any of those members are structs, then those members will remain structs.

	contract C {
		struct S { int a; bool b; }

		S public s;

		function foo() public {
			(int a, bool b) = this.s();
		}
	}

Also, the accesor function should be declared `external` and therefore not accessible as an internal function call.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 15:43:36 +0000 UTC
    </div>
</div>

