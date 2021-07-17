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
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1548" class=".btn">#1548</a>
            </td>
            <td>
                <b>
                    Remove pip imports in favor of importlib_metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This uses the backported `importlib_metadata` module to scan for installed packages instead of importing pip, which should remove the dependency on pip < 10. As of Python 3.9 it is equivalent to using `importlib.metadata`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 21:45:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1547" class=".btn">#1547</a>
            </td>
            <td>
                <b>
                    Python packaging and uploading to PyPI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains the building and publishing of the Python package of Plenum to PyPI.
A successful test tun of the PR can be found in this [GHA run](https://github.com/udosson/indy-plenum/actions/runs/1037939572). For testing purposes, the indy-plenum package was published to [TestPyPi](https://test.pypi.org/simple/). The indy-plenum package of the test can be installed via `python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple indy-plenum==1.13.0.dev133`.

@ryjones could you create a secret called `PYPI_API_TOKEN` according to[ PyPI docs](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github), please? This is needed to publish the package to PyPI. Thanks!

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 15:35:10 +0000 UTC
    </div>
</div>

