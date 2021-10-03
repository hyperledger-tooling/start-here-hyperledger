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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-3: Remove CI files used by Jenkins
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CI will be handled by Github Actions.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 21:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    Correctly handle NotFound for prefix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change correctly handles the `NotFound` error if the prefix provided to the leaves method specifies a non-existent branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 20:34:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Return InvalidStateError on NotFound
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change modifies the KV-implementation of `MerkleStateLeafReader` to return an `InvalidStateError` if a `NotFound` error is encountered.

This allows for differentiated handling of the two cases during consumption of the iterator.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 19:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    Add GHA files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These workflows are intended to replace the operations in
the Jenkinsfile.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 19:10:44 +0000 UTC
    </div>
</div>

