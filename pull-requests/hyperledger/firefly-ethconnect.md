---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/220" class=".btn">#220</a>
            </td>
            <td>
                <b>
                    Correct the Upsert syntax for MongoDB overwrite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a still using Mongo DB (rather than the lighter weight / faster LevelDB option) for receipt stores, they will see the following error when receipts are inserted into the store, after upgrading to https://github.com/hyperledger/firefly-ethconnect/releases/tag/v3.2.2:

```
[2022-05-27T10:53:11.175-04:00]  INFO Received reply message. requestId='5fcc8464-17f5-4d8a-78ad-da554a7d388d' reqOffset='' type='TransactionFailure': 0xa8c748db42ca12662a4a94f3a23c4123712378e150ef847201a8c72980eb131a
[2022-05-27T10:53:11.175-04:00] ERROR 5fcc8464-17f5-4d8a-78ad-da554a7d388d: addReceipt attempt: 1 failed, err: reflect.Value.Interface: cannot return value obtained from unexported field or method
[2022-05-27T10:53:11.175-04:00]  INFO 5fcc8464-17f5-4d8a-78ad-da554a7d388d: Waiting 0.50s before re-attempt:1 mongo write
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 14:59:42 +0000 UTC
    </div>
</div>

