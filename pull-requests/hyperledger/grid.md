---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1364" class=".btn">#1364</a>
            </td>
            <td>
                <b>
                    Add `update_batch_status` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds an operation to update a batch's batch status. This operation updates the `batch_statuses` table as well as updating any associated transaction receipts. This also updates the batch tracking migrations to automatically generate timestamps which greatly simplifies this and other operations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 17:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1363" class=".btn">#1363</a>
            </td>
            <td>
                <b>
                    Add release notes for v0.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-3</span>
            </td>
            <td>
                Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-31 16:41:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1362" class=".btn">#1362</a>
            </td>
            <td>
                <b>
                    Tag images nightly instead of main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These images are published on a nightly schedule and not on every merge
so `main` tag is incorrect.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 20:33:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1361" class=".btn">#1361</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: Update grid integration test cache dirs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the tests used $CARGO_MANIFEST/tmp as a temporary directory
by default. This change updates the tests to instead create and use a
dir grid-integration-tests/ in the standard Rust environment temp
directory.

This change also updates the tests to optionally use an environment
variable for the cache directory, and updates the test dockerfile to set
the variable to /var/cache/grid. This should allow CI to persist the
cache from a stable and standard location between runs.

Signed-off-by: Lee Bradley <bradley@bitwise.io>

Backport of: https://github.com/hyperledger/grid/pull/1305
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:58:01 +0000 UTC
    </div>
</div>

