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
                PR <a href="https://github.com/hyperledger/grid/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    Avoid duplicate events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces an EventProcessors struct to manages that event processors are only created once per circuit/service instance.

It also introduces a work-around for an issue with database transaction creation while handling commit events. It serializes the events received from event processors into a channel and handle the events serially.  This fix ensures that duplicate events won't result in duplicate entries in the DB.  This second commit may be rolled back when a proper fix for transactions is introduced.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 20:35:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    Fix 1.54.0 lint for Grid 0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This includes several commits to address lint warnings that were introduced in Rust 1.54.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 17:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/891" class=".btn">#891</a>
            </td>
            <td>
                <b>
                    Add Cylinder JWT support to app auth handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes various updates to support the authorization requirements in Splinter 0.5. This updates the Splinter dep, and various others in support of this update, to 0.5 within the Grid daemon. Authorization, in the form of Cylinder JWTs, has been added to all requests sent to the Splinter backend. This also updates the Signer used by the app auth handler to a Cylinder signer, allowing the JWT to be formed from this signer and added to rest requests. 

This functionality is behind the experimental `cylinder-jwt-support` feature. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-03 14:09:35 +0000 UTC
    </div>
</div>

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

