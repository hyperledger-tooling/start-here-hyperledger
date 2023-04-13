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
                PR <a href="https://github.com/hyperledger/solang/pull/1268" class=".btn">#1268</a>
            </td>
            <td>
                <b>
                    Disallow dynamic arrays for account metas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Account metas do not support dynamic arrays and we do not inform that to the user.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 21:57:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    Test large github runners
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
        Created At 2023-04-12 15:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1266" class=".btn">#1266</a>
            </td>
            <td>
                <b>
                    Remove redundancies in `is_next_reachable()`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After merging #1260 , I noticed the checks in my code were redundant.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 15:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1260" class=".btn">#1260</a>
            </td>
            <td>
                <b>
                    Ensure that the last instruction of a block is reachable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR supersedes #1257.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 17:28:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1259" class=".btn">#1259</a>
            </td>
            <td>
                <b>
                     Parse error definitions and revert with custom errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are not supported on Solana or Substrate, however this will help
with testing sema with evm solidity contracts.

This changes `revert()` from an builtin expression to a statement type. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-08 17:19:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1258" class=".btn">#1258</a>
            </td>
            <td>
                <b>
                    codegen::Expression should have named fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Only changes in the syntax for `codegen::Expression`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 17:20:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1256" class=".btn">#1256</a>
            </td>
            <td>
                <b>
                    v0.2.3 Geneva
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Added
- The Solana units `sol` and `lamports` are now supported, e.g. `10 sol` and `100 lamports`.
  [seanyoung](https://github.com/seanyoung)
- User defined operators are now supported. This is a feature in Ethereum Solidity v0.8.19.
  [seanyoung](https://github.com/seanyoung)
- **Solana**: if a contract uses the `SystemAccount`, `ClockAccount`, or other standard builtin
  accounts, then this is automatically added to the IDL. [LucasSte](https://github.com/LucasSte)
- **Substrate**: The content of the debug buffer is formatted in a human readable way. This vastly improves it's readability, allowing to spot API runtime return codes, runtime errors and debug prints much easier. [salaheldinsoliman](https://github.com/salaheldinsoliman) 

### Fixed
- Solana: contracts with a seed for the constructor do not require a signer in the Anchor IDL
  [seanyoung](https://github.com/seanyoung)
- Fix panic when lexing ".9" at the beginning of a file. [seanyoung](https://github.com/seanyoung)
- Forbid ABI encoding and decoding of recursive types. [xermicus](https://github.com/xermicus)
- Treat enums as 8bit uint in constant hashing. [xermicus](https://github.com/xermicus)
- Fix compilation failure with -g for the substrate target. [salaheldinsoliman](https://github.com/salaheldinsoliman)
- Fixed incorrect ABI encoding for user defined types. [xermicus](https://github.com/xermicus)  [seanyoung](https://github.com/seanyoung)
- Fixed incorrect ABI encoding for struct with fields of type `bytesN` [xermicus](https://github.com/xermicus)
- Fixed incorrect handling of recursive struct fields. [xermicus](https://github.com/xermicus)
- Fixed a bug in our Common Subexpression Elimination optimization pass [LucasSte](https://github.com/LucasSte)
### Changed
- Math overflow is now always enabled, unless the math happens with an `unchecked { .. }` block.
  The `--math-overflow` command line option has been removed. [seanyoung](https://github.com/seanyoung)
- **Substrate**: the SCALE encoder and decoder now uses a much better implementation written in our
  CFG intermediate format. [xermicus](https://github.com/xermicus)
- **Substrate**: When instantiating a new contract without providing a salt, the salt we be derived from the output of the new `instantiation_nonce` runtime API. [xermicus](https://github.com/xermicus)
- Minimal Supported Rust Version is `1.65.0`
- No longer silently overwrite contract artifacts, if the same contract is defined more than once in different locations [seanyoung](https://github.com/seanyoung)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 13:38:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1255" class=".btn">#1255</a>
            </td>
            <td>
                <b>
                    Rename Complement to BitwiseNot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BitwiseNot is a much better name.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 13:01:18 +0000 UTC
    </div>
</div>

