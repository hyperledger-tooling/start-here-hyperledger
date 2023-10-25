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
                PR <a href="https://github.com/hyperledger/solang/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    Remove balance, transfer, and send from Solana
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
        Created At 2023-10-24 21:51:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    v0.3.3: Atlantis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This release improves the Solana developer experience, since now required
accounts can be specified using annotations. For Polkadot, compatibility with
Ethereum Solidity has been increased further, it is now possible to write
[EIP-1967](https://eips.ethereum.org/EIPS/eip-1967) compatible proxy contracts.
There are many fixes all over the code base.

### Added
- **Solana** the required accounts for instructions can now be specified using function annotations. [LucasSte](https://github.com/LucasSte)
  ```
  contract Foo {
      @account(oneAccount)
      @signer(mySigner)
      @mutableAccount(otherAccount)
      @mutableSigner(otherSigner)
      function bar() external returns (uint64) {}
  }
  ```
- The language server can now format Solidity source code using the `forge-fmt` crate. [chioni16](https://github.com/chioni16)
- The langauge server can now do go references, go to implementation, and go to type
  definition. [chioni16](https://github.com/chioni16)
- **Polkadot** `Panic` errors can now be caught in try-catch statements [xermicus](https://github.com/xermicus)
- **Polkadot** custom errors are now supported [xermicus](https://github.com/xermicus)
- **Polkadot** now supporting the `address.code` builtin [xermicus](https://github.com/xermicus)

### Fixed
- **Solana** the data field of AccountInfo can now be modified. [LucasSte](https://github.com/LucasSte)
- The vscode extension now uses the solang binary in the path, if available. [seanyoung](https://github.com/seanyoung)
- Fixed a bug in the ABI encoding of dynamic arrays. [xermicus](https://github.com/xermicus)
- Fixed a bug where loading from a storage struct member was not considered a storage read.
  [xermicus](https://github.com/xermicus) [seanyoung](https://github.com/seanyoung)
- Fixed a compiler crash caused by chained assignments like `return a = b`.  [xermicus](https://github.com/xermicus)
- Variables declared in the return parameters no longer ignore the `storage` location. [xermicus](https://github.com/xermicus)

### Changed
- **BREAKING:** **Solana** the contract Solidity type can no longer be used. This type
  used to represent a single address, but this does not make sense as there are many
  accounts associated with a contract call. [LucasSte](https://github.com/LucasSte)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-22 14:44:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1572" class=".btn">#1572</a>
            </td>
            <td>
                <b>
                    Fix slice length
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When converting [this example](https://github.com/solana-developers/program-examples/blob/main/tokens/pda-mint-authority/solang/solidity/pda-mint-authority.sol) to the new Solidity annotation syntax, I uncovered a small bug in slice creation, in which we were not casting the length to `uint64`, leading to an `InvalidLength` error in Solana's runtime.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 20:04:20 +0000 UTC
    </div>
</div>

