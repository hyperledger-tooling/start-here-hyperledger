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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/769" class=".btn">#769</a>
            </td>
            <td>
                <b>
                    Fix Pike update ops for Sawtooth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes the update_* operations for the Pike module to properly set
the `end_commit_num` for the record being updated. Previously, the
`end_commit_num` was not being updated because the diesel query builder
was not properly checking for the `service_id` or lack thereof.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 21:52:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/768" class=".btn">#768</a>
            </td>
            <td>
                <b>
                    Update release notes to include bug fix
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
        Created At 2021-06-17 21:07:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/767" class=".btn">#767</a>
            </td>
            <td>
                <b>
                    Fix 1.53.0 lints
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
        Created At 2021-06-17 20:03:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    Update header copyright
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This file was updated in 2021 but the header was not updated

Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 18:31:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/765" class=".btn">#765</a>
            </td>
            <td>
                <b>
                    Daemon feature cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes changes necessary to remove "experimental" dependency between the daemon and the sdk.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 18:13:41 +0000 UTC
    </div>
</div>

