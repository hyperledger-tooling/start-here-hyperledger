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
                    
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.3.2
                </span>
            </td>
            <td>
                

The language server is much improved, and many fixes all over.

### Added
- Go to definition is now implemented in the language server.
[chioni16](https://github.com/chioni16)
- The parser has been updated to be compatible with Ethereum Solidity
v0.8.21. [seanyoung](https://github.com/seanyoung)

### Fixed
- **breaking** Resolving import paths now matches solc more closely, and
only resolves relative paths when specified as `./foo` or `../foo`.
[seanyoung](https://github.com/seanyoung)
- **Solana** The `lamports` and `data` fields of `tx.accounts` can be
modified again. [LucasSte](https://github.com/LucasSte)
- It is not longer necessary to save a Solidity file, in order for the
language server to pick up changes to the file.
[chioni16](https://github.com/chioni16)
- The negate operator `-` now checks for overflow at runtime, and other
math overflow fixes. [seanyoung](https://github.com/seanyoung)

### Changed
- The Substrate target has been renamed to Polkadot.
[xermicus](https://github.com/xermicus)
- **Polkadot** `assert()` and `require()` is now implemented as a
transction revert, rather than a trap. The error data is returned, and
encoded the same as on Ethereum. Error data is now passed to the calling
contract, all the way up the call stack.
[xermicus](https://github.com/xermicus)
- **Polkadot** constructor can be non-payable.
[xermicus](https://github.com/xermicus)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/solang/releases/tag/v0.3.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-08-24 09:44:40 +0000 UTC
    </span>
</div>

