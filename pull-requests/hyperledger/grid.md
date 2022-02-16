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
                PR <a href="https://github.com/hyperledger/grid/pull/1312" class=".btn">#1312</a>
            </td>
            <td>
                <b>
                    Add prerequisites to readme build instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are a number of libraries unlikely to be present on reader's
systems that must be installed before `cargo build` will successfully
build the project. These changes clarify prerequisites so that readers
following the README build instuctions can successfully build the
project without hitting roadblocks or guessing Grid's dependencies.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 16:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1311" class=".btn">#1311</a>
            </td>
            <td>
                <b>
                    Add dlt polling monitor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds the dlt polling monitor to Grid as an experimental
feature.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 15:20:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1310" class=".btn">#1310</a>
            </td>
            <td>
                <b>
                    Remove unused `sawtooth` module/feature in cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes the unused `sawtooth` module and feature from the CLI. The
original functionality intended to be housed in this module is handled
elsewhere.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 20:20:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1307" class=".btn">#1307</a>
            </td>
            <td>
                <b>
                    Replace node-sass@4.13.1 with sass@1.49.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change replaces node-sass due to a dependabot alert of
vulnerability CVE-2020-24025, where certificate validation was disabled
when requesting binaries.

Since node-sass is deprecated, it was replaced with sass.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 16:03:45 +0000 UTC
    </div>
</div>

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

