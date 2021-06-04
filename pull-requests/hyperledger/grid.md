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
                PR <a href="https://github.com/hyperledger/grid/pull/735" class=".btn">#735</a>
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
                `Key` option help information updated to include GRID_DAEMON_KEY and
CYLINDER_PATH defaults. `service_id` option help was updated to include
GRID_SERVICE_ID environment variable. URL option help was updated to
include GRID_SERVICE_ENDPOINT default.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 12:44:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/734" class=".btn">#734</a>
            </td>
            <td>
                <b>
                    Remove redundant service-id option at subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed that this implementation was duplicating already existing code
at the parent subcommand, so it was redundant and therefore removed.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 12:38:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/733" class=".btn">#733</a>
            </td>
            <td>
                <b>
                    Update CLI PO create to include not-draft option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Man page specifies that there would be both a draft - which is by
default, and a not-draft flag. Updated this implementation to match the
man-page, because draft is a flag and is set to true by default, there
would be no way of setting it to false. Also draft and not-draft is
the convention used for other components. This method is not yet
implemented so it should have no impact on the application.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 12:38:07 +0000 UTC
    </div>
</div>

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

