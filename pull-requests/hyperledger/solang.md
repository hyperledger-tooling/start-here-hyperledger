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
                PR <a href="https://github.com/hyperledger/solang/pull/1440" class=".btn">#1440</a>
            </td>
            <td>
                <b>
                    Bump should be hashed by last
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
        Created At 2023-07-12 18:38:16 +0000 UTC
    </div>
</div>

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

