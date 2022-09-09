---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    Fix a gh-action issue in #472
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In #472, the tox github action plugin was not configued correctly.

That results some missing code format problems in the following PRs.

This PR adds the correct configuration to tox.ini file and fixes the 
missed code format problems.

Signed-off-by: Xichen Pan <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 01:22:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    Allow docker-agent to update node config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implement the methods to request docker-agent to update config,
and restart the node.

Also fix a bug in node APIs that disallows the JSON post request.

Signed-off-by: Xichen Pan <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 12:25:56 +0000 UTC
    </div>
</div>

