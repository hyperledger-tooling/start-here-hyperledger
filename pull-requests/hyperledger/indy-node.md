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

