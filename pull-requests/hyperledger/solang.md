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
                PR <a href="https://github.com/hyperledger/solang/pull/1485" class=".btn">#1485</a>
            </td>
            <td>
                <b>
                    Avoid overflow in transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `address.transfer` and `address.send` utilize `void sol_transfer` from `solana.c` under the hood, which was saving the overflowed valued to the account balance. This PR fixes such an issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 17:56:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1483" class=".btn">#1483</a>
            </td>
            <td>
                <b>
                    Use Ubuntu 20.04 rather than 22.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've had a few users reporting that solang does not work in their environment; usually this is ubuntu 20.04 WSL.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 08:00:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1482" class=".btn">#1482</a>
            </td>
            <td>
                <b>
                    Polkadot: Integration tests use Polkadot v1.0.0 node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update integration tests to use the latest CI node build containing a substrate node built against `polkadot-v1.0.0`.

Some tests required changes in their weight calculations.

I allowed to take some shortcuts with upgrading the subxt tests. Because we have a student working on making the extrinsics library from cargo-contract re-usable, it'd be a waste spending too much time there (plan is to then use this in the CLI and the integration).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 10:58:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1481" class=".btn">#1481</a>
            </td>
            <td>
                <b>
                    Improve math tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the overflowing error in an a math overflowing tests that was not supposed to overflow and exchanges `pow`/`truncate_biguint` by `modpow`, which is more efficient.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-08 20:20:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1478" class=".btn">#1478</a>
            </td>
            <td>
                <b>
                    Fix incorrect deserialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The deserialization of `struct TokenAccountData` in the Solana library is incorrect. This PR fixes the issue and tests the deserialization of both `struct TokenAccountData` and `struct MintAccountData`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 21:52:16 +0000 UTC
    </div>
</div>

