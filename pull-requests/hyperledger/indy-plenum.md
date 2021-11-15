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

