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
                PR <a href="https://github.com/hyperledger/fabric/pull/4585" class=".btn">#4585</a>
            </td>
            <td>
                <b>
                    change evaluate RequestId for update config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the documentation and in the examples, the channel update transaction is send to one and only one orderer. Like in raft. The smartbft features are not used.

What's happening?
When an orderer receives a channel update transaction, it takes the current channel config and applies the update to it and re-signs the transaction. It then sends it to the smartbft consensus. Total 7 different transactions appear in the consensus.

My current solution fixes the error. RequestID will be calculated differently for channel update transactions.

After this change, the channel update can be sent out as a bft.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-27 05:01:51 +0000 UTC
    </div>
</div>

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

