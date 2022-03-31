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
                PR <a href="https://github.com/hyperledger/grid/pull/1362" class=".btn">#1362</a>
            </td>
            <td>
                <b>
                    Tag images nightly instead of main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These images are published on a nightly schedule and not on every merge
so `main` tag is incorrect.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 20:33:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1361" class=".btn">#1361</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: Update grid integration test cache dirs
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

Backport of: https://github.com/hyperledger/grid/pull/1305
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 14:58:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1359" class=".btn">#1359</a>
            </td>
            <td>
                <b>
                    Publish multi arch images
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
        Created At 2022-03-28 20:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1358" class=".btn">#1358</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: Add handling for Splinter error responses
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
        Created At 2022-03-28 19:03:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1357" class=".btn">#1357</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: Replace node-sass@4.13.1 with sass@1.49.7
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
        Created At 2022-03-28 18:59:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1356" class=".btn">#1356</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: Add prerequisites to readme build instructions
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
        Created At 2022-03-28 18:58:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1355" class=".btn">#1355</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: Replace tempdir library with tempfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace tempdir library with tempfile:3 because tempdir is no longer
maintained. See advisory: https://rustsec.org/advisories/RUSTSEC-2018-0017

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 18:56:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1354" class=".btn">#1354</a>
            </td>
            <td>
                <b>
                    BACKPORT 0.3: Bump dirs library from 0.3 -> 0.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Latest version of dirs adds support for XDG_DATA_HOME.

Signed-off-by: Lee Bradley [bradley@bitwise.io](mailto:bradley@bitwise.io)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 18:54:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1353" class=".btn">#1353</a>
            </td>
            <td>
                <b>
                    Add `DELAYED` batch status type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a batch status variant: `DELAYED` to the `BatchStatus` enum.
    This type will be used when a batch cannot be resubmitted quite yet but
    should be queued to do so once any prerequisites are met.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 18:22:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1352" class=".btn">#1352</a>
            </td>
            <td>
                <b>
                    Add files to build grid-dev with Github Actions
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
        Created At 2022-03-25 20:42:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1351" class=".btn">#1351</a>
            </td>
            <td>
                <b>
                    Add `get_batch_status` db operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements the `get_batch_status` operation for the Batch Tracking
    store. This operation returns the current batch status for a batch with
    a given ID and service ID. This PR also contains several other small but
    necessary updates to the models to make this work.
    
    Signed-off-by: Davey Newhall <newhall@bitwise.io>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:15:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1350" class=".btn">#1350</a>
            </td>
            <td>
                <b>
                    Add GHA to label pull requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding the backport-triage label to new pull requests will help ensure
that changes are backported when appropriate.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 20:47:53 +0000 UTC
    </div>
</div>

