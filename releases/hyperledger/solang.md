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
                    v0.3.3: Atlantis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.3.3
                </span>
            </td>
            <td>
                This release improves the Solana developer experience, since now required
accounts can be specified using annotations. For Polkadot, compatibility with
Ethereum Solidity has been increased further, it is now possible to write
[EIP-1967](https://eips.ethereum.org/EIPS/eip-1967) compatible proxy contracts.
There are many fixes all over the code base.
    
### Added
- **Solana** the required accounts for instructions can now be specified
  using function annotations. [LucasSte](https://github.com/LucasSte)
  ```
  contract Foo {
      @account(oneAccount)
      @signer(mySigner)
      @mutableAccount(otherAccount)
      @mutableSigner(otherSigner)
      function bar() external returns (uint64) {}
  }
  ```
- The language server can now format Solidity source code using the
  `forge-fmt` crate. [chioni16](https://github.com/chioni16)
- The langauge server can now do go references, go to implementation, and go to type
  definition. [chioni16](https://github.com/chioni16)
- **Polkadot** `Panic` errors can now be caught in try-catch statements
  [xermicus](https://github.com/xermicus)
- **Polkadot** custom errors are now supported
  [xermicus](https://github.com/xermicus)
- **Polkadot** now supporting the `address.code` builtin
  [xermicus](https://github.com/xermicus)
    
### Fixed
- **Solana** the data field of AccountInfo can now be modified.
  [LucasSte](https://github.com/LucasSte)
- The vscode extension now uses the solang binary in the path, if
  available. [seanyoung](https://github.com/seanyoung)
- Fixed a bug in the ABI encoding of dynamic arrays.
  [xermicus](https://github.com/xermicus)
- Fixed a bug where loading from a storage struct member was not
  considered a storage read. [xermicus](https://github.com/xermicus) [seanyoung](https://github.com/seanyoung)
- Fixed a compiler crash caused by chained assignments like `return a = b`. [xermicus](https://github.com/xermicus)
- Variables declared in the return parameters no longer ignore the `storage` location. [xermicus](https://github.com/xermicus)
    
### Changed
- **BREAKING:** **Solana** the contract Solidity type can no longer be used. This type
  used to represent a single address, but this does not make sense asthere are many
  accounts associated with a contract call. [LucasSte](https://github.com/LucasSte)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/solang/releases/tag/v0.3.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-26 15:13:24 +0000 UTC
    </span>
</div>

