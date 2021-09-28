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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Release notes for 0.3.10
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
        Created At 2021-09-24 21:29:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/198" class=".btn">#198</a>
            </td>
            <td>
                <b>
                    Remove CI files used by Jenkins
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
        Created At 2021-09-24 19:00:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Correct feature guard for serde_derive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change corrects the feature guard for serde_derive to "serde_derive", making it less dependent on the feature defined in
libtransact's Cargo.toml, and merely dependent on whether or not the optional dependency is included in the set of active features.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 21:16:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Release notes for 0.3.9
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
        Created At 2021-09-23 19:31:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    Remove StateDatabaseError::InternalError variant
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the StateDatabaseError InternalError variant, as this is a backwards-incompatible change.

In order to remove this, the original Node implementation has been restored in the kv module, the state::merkle::node::Node implementation has been reduced to only what the SQL implementation requires, and is guarded by the "state-merkle-sql" feature.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 18:27:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Restrict just doc to published configuration 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change restricts the `just doc` task to only apply the rustdoc configuration that would be run for the published crates.  Prior to this commit, `just doc` would run the whole workspace, which causes file name conflicts between libtransact and transact-cli.

Also fixes some resulting warnings from this change.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 22:27:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    SqlMerkleState typo fixes
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
        Created At 2021-09-22 19:01:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Remove outdated comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes an outdated comment, left over from the development process.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 17:51:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Correct feature guard for diesel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change corrects the feature guard for diesel to "diesel", making it less dependent on the feature defined in libtransact's Cargo.toml, and merely dependent on whether or not the optional dependency is included in the set of active features.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 15:42:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    SqlMerkleState integration test re-org
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR moves some use statements, statics and functions around, for consistent file organization.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 14:28:15 +0000 UTC
    </div>
</div>

