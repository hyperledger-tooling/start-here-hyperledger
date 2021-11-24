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
                PR <a href="https://github.com/hyperledger/indy-test-automation/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    removed circular dependencies and generalized for ubuntu 16.04 and 20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR separated the `sovrin` specific tets from indy-node tests. This removes the circular dependencies mentioned in #102.

Also, the scripts have been adjusted to run locally as well on GitHub Actions pipelines. 
The basis for testing `ubuntu 20.04` based `indy-node` artifacts is implemented. 
Current issue: There is no working `systemd` image for `ubuntu 20.04` 

A successful run of all tests in GHA can be found at: https://github.com/udosson/indy-node/actions/runs/1495380875


Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 14:41:02 +0000 UTC
    </div>
</div>

