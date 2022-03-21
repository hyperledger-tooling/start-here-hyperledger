---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    Improve snapshot creation safety
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make sure a raftpb.EntryConfChange entry does not create a snapshot with an empty block.

Also get rid of a few warning (unhandled error, context leak).

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 12:59:06 +0000 UTC
    </div>
</div>

