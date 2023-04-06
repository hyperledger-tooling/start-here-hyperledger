---
layout: default
title: solang
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Geneva
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.2.3
                </span>
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
    <a href="https://github.com/hyperledger/solang/releases/tag/v0.2.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-04-06 17:55:31 +0000 UTC
    </span>
</div>

