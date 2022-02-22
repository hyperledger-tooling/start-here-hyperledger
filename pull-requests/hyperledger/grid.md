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
                PR <a href="https://github.com/hyperledger/grid/pull/1313" class=".btn">#1313</a>
            </td>
            <td>
                <b>
                    Add `BatchBuilder` struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a `BatchBuilder` struct and implementation to mirror the Grid
structs in other modules. This also updates the `Batch` struct's fields
to be private with public accessor methods, also to mirror other
modules.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 20:21:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1312" class=".btn">#1312</a>
            </td>
            <td>
                <b>
                    Add prerequisites to readme build instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are a number of libraries unlikely to be present on reader's
systems that must be installed before `cargo build` will successfully
build the project. These changes clarify prerequisites so that readers
following the README build instuctions can successfully build the
project without hitting roadblocks or guessing Grid's dependencies.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 16:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1311" class=".btn">#1311</a>
            </td>
            <td>
                <b>
                    Add dlt polling monitor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds the dlt polling monitor to Grid as an experimental
feature.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 15:20:32 +0000 UTC
    </div>
</div>

