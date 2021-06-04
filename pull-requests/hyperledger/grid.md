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
                PR <a href="https://github.com/hyperledger/grid/pull/732" class=".btn">#732</a>
            </td>
            <td>
                <b>
                    Move `clear_database` fns to new `testing` module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the `clear_database` functions for clearing the postgres and
sqlite databases to a new testing module. These are guarded behind new
features `test-postgres` and `test-sqlite` respectively. This does not
change any functionality.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 21:14:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/729" class=".btn">#729</a>
            </td>
            <td>
                <b>
                    Update help with env var defaults
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Key` option help information updated to include GRID_DAEMON_PATH and
CYLINDER_PATH defaults. `service_id` option help was updated to include
GRID_SERVICE_ID environment variable. `url` option help was updated to
include GRID_SERVICE_ENDPOINT default.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 13:23:51 +0000 UTC
    </div>
</div>

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

