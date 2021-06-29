---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Support multiple trees with a single backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the SqlMerkleState to support the use of multiple trees in a single backend.  This is accomplished by introducing a `merkle_radix_tree` table and added a `tree_id` reference to the existing tables.  `SqlMerkleState` structs must now be constructed via a builder.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 02:25:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    Fix lint introduced with Rust 1.53.0 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 15:30:13 +0000 UTC
    </div>
</div>

