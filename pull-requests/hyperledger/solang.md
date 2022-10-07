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
                PR <a href="https://github.com/hyperledger/solang/pull/1035" class=".btn">#1035</a>
            </td>
            <td>
                <b>
                    allow constructor names in substrate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">substrate</span>
            </td>
            <td>
                This changes a few things regarding constructor names for the substrate target:

- Constructors may now have a name, like functions.
- If they have no name, `new` will be used automatically.
  - It is a convention to call "constructors" `new` in Rust too
  - `new` is a reserved keyword in Solidity, so you can't write a function called `new` anyways (prevents conflicts)
- It works nicely together with the function name mangling.

To make instantiation of `ink!` (Substrate) contracts possible in the future, I think  generating interface files is the better solution than changing our syntax to allow it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 14:34:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1034" class=".btn">#1034</a>
            </td>
            <td>
                <b>
                    Match Anchor contract deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                - Single program per Solidity contract
- Data account is created by the program, not the caller
- Seeds/bump are passed as arguments or doc comments

New syntax:
```
/** @program_id AddressLookupTab1e1111111111111111111111111 */
contract c {
      /** 
        * @seed "meh" 
        * @seed a_seed
        * @bump bump
        */
       constructor(bytes a_seed, byte1 bump) {}
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 13:25:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1033" class=".btn">#1033</a>
            </td>
            <td>
                <b>
                    Bump various dependencies and depend on rust 1.63.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Require rust 1.63 (needed by solana_rbpf crate, also phf requires rust 1.60.0)
- Bump dependencies
- Fix various clippies found with rust 1.65.0 beta
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 21:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1032" class=".btn">#1032</a>
            </td>
            <td>
                <b>
                    Add new solang logo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hyperledger designed a logo for us.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 09:48:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1031" class=".btn">#1031</a>
            </td>
            <td>
                <b>
                    Split integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solana integration tests and Anchor integration tests are semantically different, but run in a single GitHub runner. This PR splits them to ease debugging.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 21:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1029" class=".btn">#1029</a>
            </td>
            <td>
                <b>
                    Implement function dispatch in codegen for Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                This PR implements the function dispatch and the constructor dispatch in codegen for the Solana target. The old implementation in `src/emit/dispatch` has been moved to `src/emit/substrate/dispatch` and implemented as methods of `SubstrateTarget` because they are now Substrate specific.

There are some new instructions in the control flow graph for LLVM instructions that were exclusive to `emit`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 18:24:26 +0000 UTC
    </div>
</div>

