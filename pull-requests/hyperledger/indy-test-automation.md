---
layout: default
title: indy-test-automation
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-test-automation
---

# indy-test-automation <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-test-automation){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-test-automation/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    removed circular dependencies and adjusted to be executed in GHA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR separates the Hyperledger Indy packages from the sovrin packages. Also, the docker files and scripts are adjusted to run in GHA as well as in local environments.

A successful run of all `node-only` test can be found at: https://github.com/udosson/indy-test-automation/actions/runs/1372937579 The workflow has been moved to `indy-node`
Issue: #102 

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 14:01:36 +0000 UTC
    </div>
</div>

