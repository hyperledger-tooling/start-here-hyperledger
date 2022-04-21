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
                PR <a href="https://github.com/hyperledger/grid/pull/1389" class=".btn">#1389</a>
            </td>
            <td>
                <b>
                    Update protoc to 3.20.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 00:59:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1388" class=".btn">#1388</a>
            </td>
            <td>
                <b>
                    Undo batch_tracking migrations key changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                Previously, the migrations for the batch tracking tables were updated
to use a surrogate key composed of the id and service id due to Diesel's
incomplete support for composite foreign keys. This change switches the
primary key back to a composite primary key as well as the related
foreign keys and operations that need to filter based on those foreign
keys will use raw sql via the `sql_query` function.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 18:31:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1387" class=".btn">#1387</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-3: Add architecture check for protoc during grid-dev build
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
        Created At 2022-04-20 16:32:06 +0000 UTC
    </div>
</div>

