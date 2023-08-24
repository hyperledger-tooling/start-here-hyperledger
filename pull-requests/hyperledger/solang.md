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
                PR <a href="https://github.com/hyperledger/solang/pull/1503" class=".btn">#1503</a>
            </td>
            <td>
                <b>
                    Bugfix: Incorrect size width calculation of dynamic primitive arrays in SCALE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Calculate the size width of dynamic primitive arrays based on the array length instead of the array size.

Partially fixes #1502
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 10:28:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1501" class=".btn">#1501</a>
            </td>
            <td>
                <b>
                    Polkadot: Prevent storage initializers overwriting the contract input in scratch buf
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~~Store the contract input on the stack instead of in the scratch buffer to avoid overwriting it in the storage initializer.~~

The call to the storage initializer must happen before reading the input into the scratch buffer. Otherwise, the storage initializers can overwrite the input data in the scratch buffer.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 12:16:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1500" class=".btn">#1500</a>
            </td>
            <td>
                <b>
                    Polkadot: Do not emit the storage initializer twice 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is no need to deliberately emit the storage initializer CFG a second time. It just ends up as dead code because it's  being emitted anyways.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 09:26:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1499" class=".btn">#1499</a>
            </td>
            <td>
                <b>
                    Optimize and check dispatch CFG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The dispatch CFG were not optimized; I think this is an oversight as I don't see why they shouldn't be optimized.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 06:00:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1498" class=".btn">#1498</a>
            </td>
            <td>
                <b>
                    Remove some dead code in emit
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
        Created At 2023-08-22 14:16:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1497" class=".btn">#1497</a>
            </td>
            <td>
                <b>
                    Solana: Allow address and bytes to be used as @seed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows `address` or `bytesN` to have the @seed annotation on constructors.

        contract bar {
            @payer(wallet)
            constructor(@seed address seed, @seed bytes2 seed2, @bump byte b) {}
        }
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 09:03:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1496" class=".btn">#1496</a>
            </td>
            <td>
                <b>
                    v0.3.2 Brasília
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The language server is much improved, and many fixes all over.

### Added
- Go to definition is now implemented in the language server. [chioni16](https://github.com/chioni16)
- The parser has been updated to be compatible with Ethereum Solidity v0.8.21. [seanyoung](https://github.com/seanyoung)

### Fixed
- **breaking** Resolving import paths now matches solc more closely, and only resolves relative paths when specified as `./foo` or `../foo`. [seanyoung](https://github.com/seanyoung)
- **Solana** The `lamports` and `data` fields of `tx.accounts` can be modified again. [LucasSte](https://github.com/LucasSte)
- It is not longer necessary to save a Solidity file, in order for the language server to pick up changes to the file. [chioni16](https://github.com/chioni16)
- The negate operator `-` now checks for overflow at runtime, and other math overflow fixes. [seanyoung](https://github.com/seanyoung)

### Changed
- The Substrate target has been renamed to Polkadot. [xermicus](https://github.com/xermicus)
- **Polkadot** `assert()` and `require()` is now implemented as a transction revert, rather than a trap. The error data is returned, and encoded the same as on Ethereum. Error data is now passed to the calling contract, all the way up the call stack. [xermicus](https://github.com/xermicus)
- **Polkadot** constructor can be non-payable. [xermicus](https://github.com/xermicus)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 10:47:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1494" class=".btn">#1494</a>
            </td>
            <td>
                <b>
                    Bump crate dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update all dependencies that can be updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-19 08:06:26 +0000 UTC
    </div>
</div>

