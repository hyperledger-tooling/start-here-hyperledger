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
                PR <a href="https://github.com/hyperledger/transact/pull/350" class=".btn">#350</a>
            </td>
            <td>
                <b>
                    Fix typo in rustdoc comment for InTransactionPostgresBackend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 20:34:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/349" class=".btn">#349</a>
            </td>
            <td>
                <b>
                    Update publish dockerfile
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
        Created At 2022-05-20 20:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/348" class=".btn">#348</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-4: Add GHA for publishing tagged releases to crates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 18:08:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/347" class=".btn">#347</a>
            </td>
            <td>
                <b>
                    Backport 0-4: stabilize state traits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #344 (though not the commit which removes the feature)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 16:04:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/346" class=".btn">#346</a>
            </td>
            <td>
                <b>
                    Add GHA for 0-4 nightly builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 21:20:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/345" class=".btn">#345</a>
            </td>
            <td>
                <b>
                    Backport 0-4: Add missing v2 state trait implementations for SqlMerkleState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of PR #343 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 17:48:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/344" class=".btn">#344</a>
            </td>
            <td>
                <b>
                    Stabilize feature "state-trait"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR stabilizes the feature "state-trait" by renaming the feature to "state-in-transaction" and moving it to the "stable" meta feature.

For the main branch, these feature is removed.  The commits related to the renaming and moving it to "stable" will be back-ported to the 0-4 branch and included in a 0.4.x release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 20:35:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/343" class=".btn">#343</a>
            </td>
            <td>
                <b>
                    Add missing v2 state trait implementations for SqlMerkleState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR cleans up some use of the v2 state traits and implements them for the SQL backends that own their own connection pools.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 19:19:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    Backport 0-4: Merge state trait features and supporting commits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backports commits from #334, #337, #338, and #341
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 21:10:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Merge state-trait subfeatures into state-trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change merges all of the state-trait subfeatures into the state-trait, to be stabilized together.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 16:09:21 +0000 UTC
    </div>
</div>

