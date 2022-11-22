---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/873" class=".btn">#873</a>
            </td>
            <td>
                <b>
                    Remove mistaken msp path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 13:43:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/871" class=".btn">#871</a>
            </td>
            <td>
                <b>
                    add condition during delete self recipient key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is an issue during transfer token to the current implementation.
If a sender tries to sent all of his/her token to a receiver then the issue happen.

Conditions :
Sender need to send all of his/her token to the receiver 
Sender should not have any self Recipient Key for that token.

Error during endorsement : 
{
  status: 500,
  message: 'failed to delete the state of : DEL_STATE failed: transaction ID: dd10c301c30e4849c0d236ee778710e97a5576955726c87d1f16ed17ffc9cce0: invalid key. Empty string is not supported as a key by couchdb',
  payload: <Buffer >
}
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 07:10:05 +0000 UTC
    </div>
</div>

