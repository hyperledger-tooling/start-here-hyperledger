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
                PR <a href="https://github.com/hyperledger/grid/pull/744" class=".btn">#744</a>
            </td>
            <td>
                <b>
                    Update man pages for schema commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 20:24:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/743" class=".btn">#743</a>
            </td>
            <td>
                <b>
                    Update man pages for utility commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This includes admin, database, and keygen subcommands.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 19:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/742" class=".btn">#742</a>
            </td>
            <td>
                <b>
                    Update man pages for role commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 19:00:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/741" class=".btn">#741</a>
            </td>
            <td>
                <b>
                    Ignore test_db file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Running `cargo test` with experimental daemon features enabled generates
a sqlite `test_db` file. This file should never be checked in. This adds
that file to the .gitignore and .dockerignore files.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 18:25:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/740" class=".btn">#740</a>
            </td>
            <td>
                <b>
                    Update man pages for product commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 16:31:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    Update man pages for Organization commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 16:16:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/738" class=".btn">#738</a>
            </td>
            <td>
                <b>
                    Update man pages for PO and PO Version Commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 16:06:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/737" class=".btn">#737</a>
            </td>
            <td>
                <b>
                    Update man pages for location commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 14:52:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    Update man pages for agent commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 14:44:45 +0000 UTC
    </div>
</div>

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

