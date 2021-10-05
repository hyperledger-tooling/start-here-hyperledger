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
                PR <a href="https://github.com/hyperledger/transact/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    Backport 0-3: Add MerkleLeafIter back to public API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Back-port of #205 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 18:34:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: state-merkle-leaf-reader stabilization and bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This back-ports PRs #187, #201, and #202 to the 0-3 branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 15:18:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    Add MerkleLeafIter back to public API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change re-exports the `MerkleLeafIterator` struct as part of the public API of `transact::state::merkle`.

While this struct is not returned by any of the public functions on `MerkleState` or `MerkleRadixTree`, it was part of the public API and may be used by library consumers.

It also soft-deprecates this struct, as it should not be part of the public API in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 15:15:14 +0000 UTC
    </div>
</div>

