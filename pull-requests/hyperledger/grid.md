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
                PR <a href="https://github.com/hyperledger/grid/pull/889" class=".btn">#889</a>
            </td>
            <td>
                <b>
                    Backport: Fix lint for Rust 1.54.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a backport of PR #886 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-02 14:10:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/888" class=".btn">#888</a>
            </td>
            <td>
                <b>
                    Remove unused docker compose files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes unused docker compose files used to set up Grid with
Sawtooth and Splinter backends.

These docker compose files have been replaced by compose files in
specific `examples` modules.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 21:33:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/887" class=".btn">#887</a>
            </td>
            <td>
                <b>
                    Remove admin-keygen from CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the `admin` module from the CLI actions and deletes
the corresponding admin-keygen feature. This feature was not used by the
CLI and the `admin-keygen` command has been replaced by the `keygen`
command and its related options.

This change also removes a call to the removed command from the Splinter
example's docker compose file, as this command is already replaced by
the `keygen --system` command.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 21:26:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/886" class=".btn">#886</a>
            </td>
            <td>
                <b>
                    Fix 1.54.0 lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes several commits to fix new clippy lint errors from the Rust 1.54.0 release. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 17:33:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/885" class=".btn">#885</a>
            </td>
            <td>
                <b>
                    Keygen updates
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
        Created At 2021-07-27 20:18:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    Add REST API specification for Purchase Order
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
        Created At 2021-07-26 19:25:25 +0000 UTC
    </div>
</div>

