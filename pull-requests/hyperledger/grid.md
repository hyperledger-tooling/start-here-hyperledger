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
                PR <a href="https://github.com/hyperledger/grid/pull/1263" class=".btn">#1263</a>
            </td>
            <td>
                <b>
                    Remove actix-web default features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the actix-web dependencies used across Grid to
disable default features. As Grid's Splinter dependency uses another
version of actix-web, multiple versions of a default compression
feature were being pulled in which caused a build error pertaining to
multiple definitions of the same things across the different versions
of the brotli compression feature. As Grid does not currently use these
default compression features, it is safe to turn these features off.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 16:26:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1258" class=".btn">#1258</a>
            </td>
            <td>
                <b>
                    Update default schema dir to `/var/lib/grid/xsd`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The schema directory needs to be writable by Grid by default, which is
not necessarily the case with the previous directory of
`/usr/share/grid/xsd`. This change modifies the default to be
`/var/lib/grid/xsd`.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 21:05:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1257" class=".btn">#1257</a>
            </td>
            <td>
                <b>
                    Remove xsd files from example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes xsd files used in data validation, since these will be
provided by the downloader.

Resolves: #1247

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 18:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1256" class=".btn">#1256</a>
            </td>
            <td>
                <b>
                    Add architecture check for protoc during grid-dev builds
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
        Created At 2022-01-20 15:39:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1255" class=".btn">#1255</a>
            </td>
            <td>
                <b>
                    Fix PO migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the PO migrations by adding a new migrations file for the
0.3 version of the tables and reverts the original file back to its
original 0.2 state.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 21:07:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1252" class=".btn">#1252</a>
            </td>
            <td>
                <b>
                    Add `download-xsd` CLI command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add an XSD download CLI command, along with several utility methods for
downloading, extracting, and validating the files within the schema
archive.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 12:44:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1251" class=".btn">#1251</a>
            </td>
            <td>
                <b>
                    Add `StartWorkflowState`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a new struct to Workflow state, `StartWorkflowState`. This is specifically used to validate a user's permissions to create an object within a workflow.

Also updates the methods within the permission checker to better specify between checking a user's permission within a workflow and when entering a workflow. This updates the `check_permission_with_workflow` method to be `check_permission_within_workflow` and adds a new method, `check_permission_to_enter_workflow` which inspects a `StartWorkflowState` rather than a `WorkflowState`. 

This also updates the purchase order smart contract handler to use the correct permission checking method (the create_X actions now use the `check_permission_to_enter_workflow` method) and updates an affected test that was specifying the "create" workflow state which no longer exists in the built-in subworkflows as it was replaced by the 'start_state'
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 21:45:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1250" class=".btn">#1250</a>
            </td>
            <td>
                <b>
                    Update man page links to Grid docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the link at the end of each man page to point to 0.3 on the
Grid website. Previously, they pointed to 0.2 or 0.1 docs.

Resolves: #1228

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 20:38:37 +0000 UTC
    </div>
</div>

