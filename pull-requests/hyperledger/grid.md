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
                PR <a href="https://github.com/hyperledger/grid/pull/728" class=".btn">#728</a>
            </td>
            <td>
                <b>
                    Remove "pub use" and make all diesel modules pub(crate)
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
        Created At 2021-05-28 22:03:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    Rename a few sdk modules to their singular form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Renames products, locations, schemas to product, location, schema.

This is not intended to have any functional changes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 19:10:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Add feature guards for each REST API endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds several features which guard the REST API endpoint; this
will allow the daemon processes to individually pull in the specific
endpoints supported. It also allows enabling the underlying features
without enabling the associated endpoints.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 21:05:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Add "backend" as dependency for "rest-api-actix-web-3"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was an error in the dependency list for rest-api-actix-web-3 and
isn't intended to be a functional change (other than fixing compilation
if specifying this feature in isolation).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 21:05:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Remove newline from error in cli/action/product.rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also wrap ling at 100 characters.

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 19:56:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/723" class=".btn">#723</a>
            </td>
            <td>
                <b>
                    Small cleanups for the grid daemon
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
        Created At 2021-05-27 19:34:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Update copyright headers in `splinter` module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the copyright headers of files in the `splinter`
module to reflect the current year.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 19:34:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    Remove sqlite and postgres from rest api feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes sqlite and postgres from the sdk's rest-api-actix-web-3
feature, which will make it possible to conditionally use the sqlite or
postgresql when using the rest api.

This commit makes BatchList pub, because without pub, it would be
necessary to put a conditional of the underlying implementations being
enabled; it seems cleaner to simply make it pub since it does not seem
intentional to prevent creation of BatchList (which itself is pub).

Features are added to griddle for sqlite/postgres to pull in the
associated sdk features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 15:01:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    Rename batch submitter to backend client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The trait formerly known as "BatchSubmitter" was really a client to the backend (Sawtooth or Splinter). This gives it distinction from other batch-related functionality within the sdk and daemon.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 21:48:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Add database-* feature guards to the daemon
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds feature guards for the separate database backends to the Grid
daemon. This allows for conditional compilation of code that pertains to
database functionality. At least one active backend is required for the
daemon to work.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 19:59:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/716" class=".btn">#716</a>
            </td>
            <td>
                <b>
                    Fix lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a lint errors in the add_commit.rs file. This was just an
unused import that needed to get cleaned up.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 18:02:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/715" class=".btn">#715</a>
            </td>
            <td>
                <b>
                    Add "rest-api" feature to guard top-level module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This top-level "rest-api" feature prevents the rest_api module from
existing unless a REST API feature is enabled.

This is part of a larger effort to cleanup dependencies in the SDK.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 14:37:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/714" class=".btn">#714</a>
            </td>
            <td>
                <b>
                    Minor dependency cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains a set of trivial dependency adjustments for the SDK. This is part of a larger effort to clean up the SDK dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 14:14:49 +0000 UTC
    </div>
</div>

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

