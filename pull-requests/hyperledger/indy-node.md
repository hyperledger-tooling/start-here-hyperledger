---
layout: default
title: indy-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node
---

# indy-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1707" class=".btn">#1707</a>
            </td>
            <td>
                <b>
                    re-added the adjustment of packages for the cannonical archive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This needs to be re-added so the packages get named accordingly to the naming convention with the `python3` prefix.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 16:29:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1706" class=".btn">#1706</a>
            </td>
            <td>
                <b>
                    changed plenum version to 1.13.0.dev143 from GHA and fixed ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the version of the PyPI package of indy-plenum from 1.13.0.dev1034 (build and published by Jenkins instance of Sovrin) to version 1.13.0.dev143. This version was published in the latest successful GHA run from the master branch. The GHA run is at: https://github.com/hyperledger/indy-plenum/runs/3579890752?check_suite_focus=true

This change is the precondition to start migrating from https://repo.sovrin.org/deb/pool/xenial/ to https://hyperledger.jfrog.io/ui/native/indy/pool/xenial.
Also, this update is required to run the node system tests from https://github.com/hyperledger/indy-test-automation/ with the Debian files built and published in the new CI/CD pipeline.

Further, this PR contains some fixes for the Jenkins CI pipeline.

A successful run can be found at: https://github.com/udosson/indy-node/actions/runs/1413619194
The GHA run of this PR fails because the `build` image is updated.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 14:30:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1705" class=".btn">#1705</a>
            </td>
            <td>
                <b>
                    Baseimage 0.0.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Baseimage changes as discussed in #1684 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 08:41:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1704" class=".btn">#1704</a>
            </td>
            <td>
                <b>
                    LF Endings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in #1684
Signed-off-by: pSchlarb <p.schlarb@esatus.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 08:31:26 +0000 UTC
    </div>
</div>

