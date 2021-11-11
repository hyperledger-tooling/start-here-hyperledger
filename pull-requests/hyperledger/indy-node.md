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
                PR <a href="https://github.com/hyperledger/indy-node/pull/1713" class=".btn">#1713</a>
            </td>
            <td>
                <b>
                    bump version of indy plenum and added pypi versio to 3rd party artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR bumps the version of `Indy Plenum`  to `1.13.0.dev175`.
Also, this PR adds the most recent version names to the 3rd party artifacts.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 10:09:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1711" class=".btn">#1711</a>
            </td>
            <td>
                <b>
                    prepares indy-plenum package version of debian version depedency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change is needed to replace the PyPI version of `plenum` with the version of the Debian artifact.
Otherwise, we run into this error:
`indy-node : Depends: indy-plenum (= 1.13.0.dev169) but 1.13.0~dev169 is to be installed`

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 16:17:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1710" class=".btn">#1710</a>
            </td>
            <td>
                <b>
                    bump indy-plenum to version 1.13.0.dev169
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                bump indy-plenum to version `1.13.0.dev169`  from the most recent build at https://github.com/hyperledger/indy-plenum/actions/runs/1436144765

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 20:40:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1709" class=".btn">#1709</a>
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
                Cherry-picked commit https://github.com/hyperledger/indy-node/commit/5994b3fab897d9e8f999400607670f5228627939 from master to upgrade version of `action/setup-jfrog-ci` to `v2`.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 11:54:40 +0000 UTC
    </div>
</div>

