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
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1561" class=".btn">#1561</a>
            </td>
            <td>
                <b>
                    Bug fix: Cache of 3rd party dependencies & uploading of existing packages to PyPI 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes two things:
- The cache key of the uploading of the 3rd party dependencies (deb) was different than the one from `build_3rd_party_dependencies` --> now the same
- When re-running all jobs of the pipeline and if the python packages have already been uploaded to PyPi in the previous one this caused an error --> now fixed by `skip existing`. (Solution was provided by @WadeBarnes)

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 16:19:08 +0000 UTC
    </div>
</div>

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

