---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4584" class=".btn">#4584</a>
            </td>
            <td>
                <b>
                    fix gateway integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The default timeout for commit and approveformyorg operations on peer cli is 30 seconds.
It often happens that peer cli does not have enough time to perform these operations.
I fixed it so that this time can be passed to peer cli from integration tests.

Probably not all bugs for gateway tests are solved, but the work will be more stable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-25 16:46:22 +0000 UTC
    </div>
</div>

