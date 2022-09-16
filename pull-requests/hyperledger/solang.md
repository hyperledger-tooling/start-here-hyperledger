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
                PR <a href="https://github.com/hyperledger/solang/pull/1016" class=".btn">#1016</a>
            </td>
            <td>
                <b>
                    Release v0.1.13: TBD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                v0.1.13 Singapore

### Changed
- On Solana, emitted events are encoded with Borsh encoding following the Anchor
  format.
  [LucasSte](https://github.com/LucasSte)
- The ewasm target has been removed, since ewasm is not going to implemented on
  Ethereum. The target has been reused for an new EVM target, which is not complete
  yet.
  [seanyoung](https://github.com/seanyoung)

### Added
- Solana v1.11 is now supported.
  [seanyoung](https://github.com/seanyoung)
- On Solana, programs now use a custom heap implementation, just like on
  Substrate. As result, it is now possible to `.push()` and `.pop()` on
  dynamic arrays in memory.
  [seanyoung](https://github.com/seanyoung)
- Arithmetic overflow tests are implemented for all integer widths,
  [salaheldinsoliman](https://github.com/salaheldinsoliman)
- Add an NFT example for Solana
  [LucasSte](https://github.com/LucasSte)
- Add a wrapper for the Solana System Program
  [LucasSte](https://github.com/LucasSte)
- The selector for functions can be overriden with the `selector=hex"abcd0123"`
  syntax.
  [seanyoung](https://github.com/seanyoung)
- Shell completion is available using the `solang shell-completion` subcommand.
  [xermicus]([https://github.com/xermicus)
- Add support for the `create_program_address()` and `try_find_program_address()`
  system call on Solana
  [seanyoung](https://github.com/seanyoung)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 15:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1015" class=".btn">#1015</a>
            </td>
            <td>
                <b>
                    Refactor emit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR refactors the emit code. The largest problem there was that `emit/mod.rs` has about 10 thousand lines, making it difficult to navigate. Here is a summary of my changes:

1. The trait `TargetRuntime` only defines an interface for behaviors that are not shared between targets. All shared implementations are now standalone functions.
2. I created a `StorageSlot` to be an interface for storage management functions for environments that depend on storage slots, like Substrate and EVM.
3. Target specific code is separated into folders. Code emission for Solana is under `emit/solana` and for Substrate, under `emit/substrate`.
4. The implementation of the `TargetRuntime` trait is located in `emit/<target>/target.rs`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 18:40:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1013" class=".btn">#1013</a>
            </td>
            <td>
                <b>
                    Fix random test failure in test_mul_within_range
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If gen_biguint() generated a 0, then the sub(1) will cause the test to fail.

See https://github.com/hyperledger/solang/actions/runs/3044527275/jobs/4905014572

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 12:03:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1012" class=".btn">#1012</a>
            </td>
            <td>
                <b>
                    Add semantic information to CFG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should help @salaheldinsoliman implement overflow detection for constants in the CFG. It adds information about the origin of each instruction to the CFG. Each instruction is now classified either as from Solidity, Yul or Codegen.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 21:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1011" class=".btn">#1011</a>
            </td>
            <td>
                <b>
                    Fix function calls via contract name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Disallow direct access to functions (and constants) except for base contracts. This is not valid in `solc` but was allowed in solang.

Fixes #1007 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 12:16:22 +0000 UTC
    </div>
</div>

