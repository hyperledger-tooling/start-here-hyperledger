---
layout: default
title: zeto
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/zeto
---

# zeto <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/zeto){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Add Key mgmt library and create a top-level sparse-merkle-tree library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - moved the sparse merkle tree implementation code to a top-level package `sparse-merkle-tree`
- started a new top-level package `keys` to demonstrate usage of existing encrypted keys capabilities for the Babyjubjub curve
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-31 12:55:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Add circuits for KYC enforcement with anonymity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A sample solution that enforces KYC on the sender and receiver Babyjubjub keys, by using a merkle tree in the smart contract to capture the registered identities, so that the transactions can prove against the current merkle tree root.

> Note that the merkle tree implementation in Solidity currently only supports appending.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-30 13:07:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/zeto/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Add support for anchoring with an ERC20 contract with deposit and withdraw
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
        Created At 2024-07-25 21:56:35 +0000 UTC
    </div>
</div>

