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
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1560" class=".btn">#1560</a>
            </td>
            <td>
                <b>
                    Remove unused dockerfiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 20:33:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1559" class=".btn">#1559</a>
            </td>
            <td>
                <b>
                    Ubuntu 20.04: Publishing of Python packages to PyPI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves Issue #1555 and integrates the publishing of the Python package of Plenum to PyPI into the existing GHA workflow.

A successful run of the publishing to (Test)PyPI can be found [here](https://github.com/udosson/indy-plenum/actions/runs/1101535181).
The published Python package of Plenum can be found on Test-PyPI [indy-plenum 1.13.0.dev238](https://test.pypi.org/project/indy-plenum/1.13.0.dev238/)

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 13:17:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1558" class=".btn">#1558</a>
            </td>
            <td>
                <b>
                    set publishPackages as executable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `publishPackage` needs to be set as executable.
This PR just changes the mode of ` .github/actions/publish-deb/publishPackages` to 755.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 10:59:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1557" class=".btn">#1557</a>
            </td>
            <td>
                <b>
                    Support publishing off a development branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - For example, support publishing off the `ubuntu-20.04-upgrade` branch.
- Determine the `distribution` based on the version of Ubuntu being used for the build.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 21:34:44 +0000 UTC
    </div>
</div>

