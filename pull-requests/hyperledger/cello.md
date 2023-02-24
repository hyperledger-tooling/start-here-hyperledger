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
                PR <a href="https://github.com/hyperledger/cello/pull/520" class=".btn">#520</a>
            </td>
            <td>
                <b>
                    Allow deleting node w/o docker container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Before, trying to delete a node with no active docker container

will cause ResourceNotFound error, and the node data in database

can't be removed. Now before stopping and deleting docker containers,

check if it exists or not. If not exists, delete the node from database directly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 14:32:02 +0000 UTC
    </div>
</div>

