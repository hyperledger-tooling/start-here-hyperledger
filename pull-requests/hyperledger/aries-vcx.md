---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/903" class=".btn">#903</a>
            </td>
            <td>
                <b>
                    CI: Do not publish napi wrapper when running in fork PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Should prevent this https://github.com/hyperledger/aries-vcx/pull/884 kind of failures
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 15:46:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/902" class=".btn">#902</a>
            </td>
            <td>
                <b>
                    Feature/anoncreds rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A draft implementation of the `anoncreds-rs` crate. This PR is mainly created as a reference point for the future when the (working) implementation can be done without all kinds of crazy workarounds and code smell.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 12:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/901" class=".btn">#901</a>
            </td>
            <td>
                <b>
                    Rename tails variables in prover code
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
        Created At 2023-07-18 11:33:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/900" class=".btn">#900</a>
            </td>
            <td>
                <b>
                    Release 0.57.0
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
        Created At 2023-07-17 13:28:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/899" class=".btn">#899</a>
            </td>
            <td>
                <b>
                    Tweak CI to fix build-docker-android on main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Additional tweak to prevent CI running out of disk space
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 13:28:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    Cleanup/constant
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove unused constants
- Removed unused testing ffi method `vcx_set_next_agency_response`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 15:00:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/897" class=".btn">#897</a>
            </td>
            <td>
                <b>
                    Refactor dealing with tails_dir in tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor tests (way of creating tails directory)
- Clear up confusion calling variables `tails_file` what actually is `tails_directory`
- Remove duplicated method for creating tmp directories and files

CI: 
- Small adjustment, when building android docker image, in case of cache miss, do not try to load up `main` branch revision of that image (this is happening to optimize CI in order to reuse some docker layers)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 14:39:48 +0000 UTC
    </div>
</div>

