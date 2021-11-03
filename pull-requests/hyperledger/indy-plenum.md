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

