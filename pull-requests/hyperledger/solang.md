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
                PR <a href="https://github.com/hyperledger/solang/pull/1506" class=".btn">#1506</a>
            </td>
            <td>
                <b>
                    Require rust 1.70.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                clap, one of our dependencies, requires 1.70.0 now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 09:18:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1505" class=".btn">#1505</a>
            </td>
            <td>
                <b>
                    Fix address name mangling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There was some old code for when we were using eth abis on Solana.

Fixes https://github.com/hyperledger/solang/issues/1495
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 09:07:23 +0000 UTC
    </div>
</div>

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

