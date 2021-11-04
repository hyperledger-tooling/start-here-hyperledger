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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1570" class=".btn">#1570</a>
            </td>
            <td>
                <b>
                    added importlib-metadata as debian package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added missing 3rd party dependency `importlib-metadata` to the build process of the Debian packages.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 15:51:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1569" class=".btn">#1569</a>
            </td>
            <td>
                <b>
                    pinned dependencies because of missing support for python 3.5 and adjusted Jenkins CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pinned the following PyPI packages to specific versions that are compatible with Python 3.5 and to fix CVEs.
- `setuptools<=50.3.2`
- `pygments==2.7.4`
- `importlib-metadata==2.1.1`

Further, this PR fixes the issue of the `python` executable related to the `virtualenv` of Jenkins CI.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 09:27:18 +0000 UTC
    </div>
</div>

