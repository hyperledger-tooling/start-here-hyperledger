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
                PR <a href="https://github.com/hyperledger/solang/pull/1400" class=".btn">#1400</a>
            </td>
            <td>
                <b>
                    Runtime error strings must be LLVM constant strings instead of dynamically allocated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The contract linked at #1367 calls `vector_new` too many times, because the runtime error strings are dynamically allocated during execution. This PR makes the runtime error strings constant attributes in LLVM, so they are not allocated.

In addition, this PR has these changes:
1. The test case caused a stack overflow in constant folding, so I split `fn expression` into multiple small functions.
2. `log_runtime_error` contained repeated code for both targets and has been removed from the `trait TargetRuntime`.
3. `error_message_with_loc` now adds the new line character.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 21:26:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1397" class=".btn">#1397</a>
            </td>
            <td>
                <b>
                    Substrate: Implement builtin for `set_code_hash` API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exposes a low-level builtin function for calling `seal_set_code_hash`. The code hash arguments is of type `bytes` intentionally (and not of type `Hash`, so that it matches the the pointer expected by the API function. `Hash`, which is just an alias to `bytes32`, will internally be represented as an `i256`. I came to the conclusion that, given this type conversion can easily be written in Solidity, we do and should not want to deal with that in the compiler, be it in emit or in codegen or elsewhere. 
Instead, a more high level function, that asks for a `Hash` argument and converts that to `bytes`, should rather be implement in the substrate Solidity library (once we have it).
Additionally, if some parachain decides to use a hash longer than 32bytes, using just a `bytes` pointer will still work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 15:19:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1396" class=".btn">#1396</a>
            </td>
            <td>
                <b>
                    Add markdown formatting to hover messages
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
        Created At 2023-06-26 09:45:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1395" class=".btn">#1395</a>
            </td>
            <td>
                <b>
                    Drop diagnostics on closing the file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When closing a file in VS code, all the warnings and errors remain in the list of problems. This removes all diagnostics pertaining to the close file. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:29:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1394" class=".btn">#1394</a>
            </td>
            <td>
                <b>
                    Pick up unsaved changes in a file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently the language server reads the file, rather than using the source code which is sent to it over language server requests. In order for the language server to update with the latest text of the source file, one needs to save the file. 
These changes enable the language server to update as one types. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:26:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1393" class=".btn">#1393</a>
            </td>
            <td>
                <b>
                    add option to set trace level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows the user to configure the verbosity of trace of messages exchanged between client and the server.
The user can set this in `User Settings` (press ctrl/cmd+,) and then searching for solidity related configuration. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:23:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1392" class=".btn">#1392</a>
            </td>
            <td>
                <b>
                    add contract author and version flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements a way to specify the author and version of all contracts via the CLI or via "solang.toml"
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 02:37:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1391" class=".btn">#1391</a>
            </td>
            <td>
                <b>
                    Optimize modifier CFGs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Closes #1385 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-25 11:46:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1390" class=".btn">#1390</a>
            </td>
            <td>
                <b>
                    Substrate: Implement `delegatecall()`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Required by upgradable proxy patterns.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-24 17:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1389" class=".btn">#1389</a>
            </td>
            <td>
                <b>
                    Bump Solana, Anchor and Ubuntu
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
        Created At 2023-06-24 13:20:56 +0000 UTC
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

