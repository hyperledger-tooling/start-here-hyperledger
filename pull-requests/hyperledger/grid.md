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
                PR <a href="https://github.com/hyperledger/grid/pull/713" class=".btn">#713</a>
            </td>
            <td>
                <b>
                    Add brief CommitStore module doc comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a brief CommitStore module doc comment to the diesel commit
store mod.rs file. This also adds a doc comment explaining the
`resolve_fork` db operation.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 21:53:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/712" class=".btn">#712</a>
            </td>
            <td>
                <b>
                    Add Schema namespace to location txn inputs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was causing location transactions to fail when the smart contract
attempted to read the location schema.

Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:51:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/711" class=".btn">#711</a>
            </td>
            <td>
                <b>
                    Properly wrap lines at 100 characters in grid cli
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
        Created At 2021-05-25 19:43:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/709" class=".btn">#709</a>
            </td>
            <td>
                <b>
                    Use `optional()` method to convert results
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the commit store operations to use the `optional()` method
to handle Diesel Results. This method handles converting the results
into Options or the appropriate NotFound errors.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 20:23:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    Update Commit store errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the commit store error module. This removes the
CommitEventError error type as it was a duplicate of CommitStoreError.
This also moves the From implementations of CommitStoreError to the
error.rs file to be in line with the best practices. Lastly, this
updates the CommitStore implementations to use the From implementations.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 18:50:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/706" class=".btn">#706</a>
            </td>
            <td>
                <b>
                    Update copyright for pike modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All of these files were substantially updated in 2021 and the copyright
header needs to reflect that.

Signed-off-by: Ryan Banks <rbanks@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 16:25:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/705" class=".btn">#705</a>
            </td>
            <td>
                <b>
                    Move sdk permissions into pike/permissions module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                /sdk/src/permissions.rs was split apart into two separate files,
"/sdk/pike/permissions/mod.rs" which contains the PermissionChecker
implementation, and "/sdk/pike/permissions/error.rs" which contains the
PermissionCheckerError implementation. This means also that the import
path changed from grid_sdk::permissions to grid_sdk::pike::permissions,
so the handler files requesting permissions has also updated.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 02:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/704" class=".btn">#704</a>
            </td>
            <td>
                <b>
                    Fix typos in Pike smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes several typos present in the Pike smart contract's
`handler` module.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 20:14:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/702" class=".btn">#702</a>
            </td>
            <td>
                <b>
                    Fix  typos and formatting issues in Grid Pike smart contract
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
        Created At 2021-05-20 19:28:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    Have only one DEFAULT_GRID_PROTCOL_VERSOIN const
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Banks <rbanks@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 18:47:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/698" class=".btn">#698</a>
            </td>
            <td>
                <b>
                    Update signer to match splinter's pattern
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
        Created At 2021-05-19 19:05:16 +0000 UTC
    </div>
</div>

