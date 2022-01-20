---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2472" class=".btn">#2472</a>
            </td>
            <td>
                <b>
                    [#2471] Failed to find OpenSSL development headers on MacOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 16:02:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2470" class=".btn">#2470</a>
            </td>
            <td>
                <b>
                    Update the version of Rust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Upgrade to Rust `1.58.0`
- Update code to align with the newer coding conventions.
  - Clean up linting and compiler warnings.
- Pin `pip<21.0` and `setuptools<=50.3.2` in `libindy/ci/ubuntu.dockerfile` to resolve build/test issues on ubuntu 16.04.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>

This PR addresses the cargo resolver issues causing the the Jenkins builds to fail by updating the Rust/Cargo versions used for the builds.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 19:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2469" class=".btn">#2469</a>
            </td>
            <td>
                <b>
                    [#2468] Allow java samples to run individually & polish sample docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 11:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2466" class=".btn">#2466</a>
            </td>
            <td>
                <b>
                    [#2465] Cannot build java wrapper due to javadoc errors
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
        Created At 2022-01-17 16:08:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2462" class=".btn">#2462</a>
            </td>
            <td>
                <b>
                    Update indy-walkthrough.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This work changes "Trust Anchor" to "Endorser" to align with the changes in 79aed586c586da8d47adb423ff3f7dcbf31fcb22
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 13:31:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2461" class=".btn">#2461</a>
            </td>
            <td>
                <b>
                    [#2445] Fix build of postgres storage plugin on ARM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issue #2445 
Building the postgres storage plugin fails on ARM (tested with v7 and v8) due to a typecast error. Adjusting the type fixed the problem.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 07:55:45 +0000 UTC
    </div>
</div>

