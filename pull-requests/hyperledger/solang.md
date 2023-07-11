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
                PR <a href="https://github.com/hyperledger/solang/pull/1438" class=".btn">#1438</a>
            </td>
            <td>
                <b>
                    Create PDA hash table example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I saw an example of a PDA hash table on [Anchor's website](https://www.anchor-lang.com/docs/pdas#hashmap-like-structures-using-pd-as). I liked it and wanted to replicate it in Solidity.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 15:15:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    Update roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I changed the roadmap to reflect what we are working on right now. Calling Solidity from Rust is not even in our backlog, so I removed it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 13:17:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1432" class=".btn">#1432</a>
            </td>
            <td>
                <b>
                    Identify externally callable functions in `sema`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The information whether a given function is supposed to be reachable via an external call to the contract is currently done directly in `codegen`. However, we need this information during the ABI generation too. This fixes a bug where inherited public functions would end up duplicated in the contract metadata.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 16:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1431" class=".btn">#1431</a>
            </td>
            <td>
                <b>
                    Remove unwanted files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These files are temporary and automatically generated during tests. They have been included in the repository.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 15:47:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1427" class=".btn">#1427</a>
            </td>
            <td>
                <b>
                    Do not return arguments of revert
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves #1152. @salaheldinsoliman has already done most of the job. I certified that the parameter string in `revert` is indeed printed and removed all returns on Solana, as they have no effect (Anchor does not decode return data when a function reverts).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 21:24:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1426" class=".btn">#1426</a>
            </td>
            <td>
                <b>
                    Avoid narrowing casts from `size_t` to `uint32_t`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I changed all occurrences of `size_t` to `uint32_t`, except for `sol_memset` from `solana_sdk.h`.
Converting from `size_t` to `uint32_t` could cause an overflow on Solana.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 18:37:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1423" class=".btn">#1423</a>
            </td>
            <td>
                <b>
                    Minor code improvements (nfc)
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
        Created At 2023-07-05 11:17:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1422" class=".btn">#1422</a>
            </td>
            <td>
                <b>
                    Add Solana minimum balance library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add runtime function for calculating the balance required for instantiating a contract of a certain size.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 10:26:57 +0000 UTC
    </div>
</div>

