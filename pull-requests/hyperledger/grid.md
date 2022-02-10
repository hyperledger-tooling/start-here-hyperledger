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
                PR <a href="https://github.com/hyperledger/grid/pull/1305" class=".btn">#1305</a>
            </td>
            <td>
                <b>
                    Update grid integration test cache dirs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the tests used $CARGO_MANIFEST/tmp as a temporary directory
by default. This change updates the tests to instead create and use a
dir grid-integration-tests/ in the standard Rust environment temp
directory.

This change also updates the tests to optionally use an environment
variable for the cache directory, and updates the test dockerfile to set
the variable to /var/cache/grid. This should allow CI to persist the
cache from a stable and standard location between runs.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 20:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1297" class=".btn">#1297</a>
            </td>
            <td>
                <b>
                    Cache Grid XML in Github Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 19:20:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1296" class=".btn">#1296</a>
            </td>
            <td>
                <b>
                    Add handling for Splinter error responses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the SplinterBackendClient to so that it will
pass on error messages from Splinter error responses, and not
incorrectly mark them as internal errors.

It also adds a number of tests to verify the output in various
scenarios.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 18:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Set dotenv-load to true in justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Starting with version 0.11.0, just ignores .env files by default. This
breaks some recipes because we read docker environment variables from
the .env file.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 15:32:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Set dotenv-load to true in justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Starting with version 0.11.0, just ignores .env files by default. This
breaks some recipes because we read docker environment variables from
the .env file.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 02:39:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1287" class=".btn">#1287</a>
            </td>
            <td>
                <b>
                    Add release notes for v0.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 19:49:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    Add files for publishing a release when a tag is pushed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 19:19:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1285" class=".btn">#1285</a>
            </td>
            <td>
                <b>
                    Correct docker-compose and packaging for `/var/cache/grid`
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
        Created At 2022-02-03 18:57:28 +0000 UTC
    </div>
</div>

