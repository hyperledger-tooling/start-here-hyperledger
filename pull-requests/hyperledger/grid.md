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
                PR <a href="https://github.com/hyperledger/grid/pull/1306" class=".btn">#1306</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: move data validation tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the data_validation tests to the cli integration tests so
the XSD files can be downloaded using the `grid download-xsd` command.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 19:10:14 +0000 UTC
    </div>
</div>

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

