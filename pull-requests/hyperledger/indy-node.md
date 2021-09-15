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
                PR <a href="https://github.com/hyperledger/indy-node/pull/1699" class=".btn">#1699</a>
            </td>
            <td>
                <b>
                    Ubuntu 20.04: bug fix: added missing env of distribution in publish_artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The recently merged CI/CD pipeline in #1697 missed passing `distribution` as env variable in the `publish-artifacts` step. This PR fixes the issue so that the debian packages get uploaded to the correct directory.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 16:48:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1698" class=".btn">#1698</a>
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

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 14:24:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1697" class=".btn">#1697</a>
            </td>
            <td>
                <b>
                    Ubuntu 20.04. CI/CD Pipeline as GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves #1678 and #1679 and provides the GHA workflow for the CI and the CD pipeline of Indy-Node.
Also, this PR contains an update of the `ubuntu-20.04-upgrade` feature branch with the most recent commits of `master`.
The PR contains:
- CI workflow based on `master` branch and Indy-Plenum
- CD workflow based on `master` branch and Indy-Plenum
- Fixed linting issues with newer version of `flake8` (flake8==3.8.4) and `python 3.8`
- updated the version of Indy-SDK to `python3-indy==1.15.0-dev-1625`, the same version as used in Indy-Plenum which contains the freeze leger support.
- adjusted `runner.py` to be compatible with the newer version of `pytest` (pytest>=6.2.2)
- `install_requires` in `setup.py` is based on `indy-plenum==1.13.0.dev135` which was built and published from the `ubuntu-20.04-upgrade` branch of Indy-Plenum in this [GHA run](https://github.com/udosson/indy-node/actions/runs/1230157953)
- copied the uploading structure of the debian file to jfrog artifactory from `master` branch

A successful run of the workflow can be found at: https://github.com/udosson/indy-plenum/actions/runs/1186783441

Thanks to @WadeBarnes for all your support! 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 07:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1696" class=".btn">#1696</a>
            </td>
            <td>
                <b>
                    Update version of Indy SKD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update version of Indy SDK to the same version used in Indy-Plenum which is at `python3-indy==1.15.0-dev-1625`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 16:24:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1695" class=".btn">#1695</a>
            </td>
            <td>
                <b>
                    fix uploading of deb files with the same name but different distribution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR rearranges the uploading structure of the debian files according to the changes made in Indy-Plenum in this [commit](https://github.com/hyperledger/indy-plenum/commit/52ddd72c0dec5f037396bf0e88acbd38d13cdb4d).
The new structure prevents errors in uploading of debian files with the same filename but build from a different distribution.
The new structure will be as follows:
- `indy/pool/xenial/[dev, main, rc, stable]`
- `indy/pool/bionic/[dev, main, rc, stable]`
- `indy/pool/focal/[dev, main, rc, stable]`

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 13:19:09 +0000 UTC
    </div>
</div>

