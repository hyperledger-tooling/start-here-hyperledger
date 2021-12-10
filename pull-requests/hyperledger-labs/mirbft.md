---
layout: default
title: mirbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/mirbft
---

# mirbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/mirbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Use proper epoch numbers with checkpoint messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The epoch number of a checkpint now always corresponds to the epoch
the associated sequence number belongs to.
At epoch transition, rathen than having an epoch "end" with a checkpoint,
the next epoch "starts" with a checkpoint, and thus the checkpoint
is associated with the new epoch rather than with the old one.
This also makes more sense with respect to the associated sequence number.

Signed-off-by: Matej Pavlovic <matopavlovic@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 12:13:25 +0000 UTC
    </div>
</div>

