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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/773" class=".btn">#773</a>
            </td>
            <td>
                <b>
                    Fix typo in schema contract error msg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a typo in an error message in the schema smart contract
caused by attempting to update a smart contract with a duplicate
property.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 19:01:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/772" class=".btn">#772</a>
            </td>
            <td>
                <b>
                    Update location ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a bug in the operation to update a location in the Grid DB. This bug was causing the `end_commit_num` to not be updated. This also removes the unused `update_location` operation. Updates to locations are handled by the `add_location` operation. This is in line with the other Grid DB modules.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 17:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/771" class=".btn">#771</a>
            </td>
            <td>
                <b>
                    Add --skip flag to keygen CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                subsequent runs of docker compose up in the example projects would fail
due to keys created in previous runs. Adding a --skip flag allows us to
reuse previously-created keys. Also updated docker-compose in example
projects

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 15:54:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/770" class=".btn">#770</a>
            </td>
            <td>
                <b>
                    Fix CLI signing path for --key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                current_user_search_path() would look in root/.cylinder/keys, whereas we
have documentation that leads us to root/.grid/keys. This change aligns
code to the documentation.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 14:59:25 +0000 UTC
    </div>
</div>

