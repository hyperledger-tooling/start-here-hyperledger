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
                PR <a href="https://github.com/hyperledger/grid/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    Fix Bytea diesel type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes an issue with the `Bytea` type in diesel. This was previously
an alias to the `Binary` type but no longer exists in diesel for sqlite.
This does still exist for postgres but this was causing lint issues when
running without the postgres feature. Functionality should not change.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 14:31:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/780" class=".btn">#780</a>
            </td>
            <td>
                <b>
                    Stabilize product-gdsn
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
        Created At 2021-06-24 18:52:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/779" class=".btn">#779</a>
            </td>
            <td>
                <b>
                    Stabilize postgres features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This stabilizes the postgres database features by moving the "postgres"
sdk feature to stable and any remaining associated "database-postgres"
features in other parts of Grid to stable.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 18:20:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/778" class=".btn">#778</a>
            </td>
            <td>
                <b>
                    Stabilize sqlite features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This stabilizes the "sqlite" sdk feature by moving it into stable. This
also moves its associated "database-sqlite" feature in other parts of
Grid into stable.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 18:20:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/777" class=".btn">#777</a>
            </td>
            <td>
                <b>
                    Fix Pike SDK comment typos
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
        Created At 2021-06-23 17:24:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/776" class=".btn">#776</a>
            </td>
            <td>
                <b>
                    Add module level documentation for product-gdsn
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
        Created At 2021-06-22 21:29:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/775" class=".btn">#775</a>
            </td>
            <td>
                <b>
                    Add explanation to gdsn 3.1 grid schemas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 20:49:08 +0000 UTC
    </div>
</div>

