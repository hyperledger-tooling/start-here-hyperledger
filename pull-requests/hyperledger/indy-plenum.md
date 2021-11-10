---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1577" class=".btn">#1577</a>
            </td>
            <td>
                <b>
                    pinned version of importlib-metadata because of issue with fpm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR pins the version of `importlib-metadata` to `v3.10.01`. From version `4.0.0`  on, the resulting package ends in `python3-importlib-metadata_0.0.0_amd64.deb`.

The issue can be seen at: https://github.com/hyperledger/indy-plenum/runs/4166593170?check_suite_focus=true#step:5:5304 

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 15:47:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1576" class=".btn">#1576</a>
            </td>
            <td>
                <b>
                    added versions of 3rd party packages to Debian artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR retrieves the most recent version of the third-party dependencies and includes the version number into the name of the artifacts published to Artifactory. This is needed because without it the artifacts get published with version `0.0.0` e.g.  `python3-importlib-metadata_0.0.0_amd64.deb` (https://hyperledger.jfrog.io/ui/native/indy/pool/focal/dev/i/importlib-metadata)

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 12:10:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    updated version of setup-jfrog-cli to v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-picked commit https://github.com/hyperledger/indy-plenum/commit/765a499e5aa629261c89b6127f7e612f6dd130bf from master to upgrade version of `action/setup-jfrog-ci` to `v2`.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 11:41:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    bump version of zipp to 1.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump version of `zipp` from `1.0.0` to `1.2.0` because `zipp==1.0.0` depends on `more-itertools`. To reduce the number of dependencies this PR updates `zipp` to version `1.2.0` that doesn't depend on additional PyPI packages anymore.


Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 11:36:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1572" class=".btn">#1572</a>
            </td>
            <td>
                <b>
                    added pygments, and zipp as 3rd party artifacts and updated version o…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …f setuptools

This PR adds `pygments` and `zipp`  to the build-script of the 3rd party artifacts.
`Pygments` could probably removed in a future commit.
`zipp` is a dependency of `importlib-metadata`. In Ubuntu `focal`, `zipp` is of the Canonical archive (https://ubuntu.pkgs.org/20.04/ubuntu-main-amd64/python3-zipp_1.0.0-1_all.deb.html)

Also, this PR updates `setuptools` to the latest version with Python3.5 support

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 14:21:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1571" class=".btn">#1571</a>
            </td>
            <td>
                <b>
                    updated version of setup-jfrog-cli to v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the GitHub Action `setup-jfrog-cli` from `v1` to `v2`. The default version of the `jfrog-cli` changes from `v1.51.1` to `v2.3.0`.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 13:17:07 +0000 UTC
    </div>
</div>

