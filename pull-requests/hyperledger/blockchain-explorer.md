---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    bugfix: prevent ETIMEOUT error from shuting down explorer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## This PR:
- prevents the explorer from shutting down on `ETIMEOUT` error.

## Error stack:
```
[2021-07-21T14:26:47.644] [ERROR] FabricGateway - Failed to get chain info from channel defaultchannel :  FabricError: Query failed. Errors: ["Error: 13 INTERNAL: Received RST_STREAM with code 2 triggered by internal client error: read ETIMEDOUT"]
    at SingleQueryHandler.evaluate (.../blockchain-explorer/node_modules/fabric-network/lib/impl/query/singlequeryhandler.js:47:23)
    at processTicksAndRejections (internal/process/task_queues.js:97:5)
    at async Transaction.evaluate (.../blockchain-explorer/node_modules/fabric-network/lib/transaction.js:276:25)
[2021-07-21T14:26:47.644] [INFO] SyncServices - syncBlocks: Failed to retrieve channelInfo >> defaultchannel
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 10:45:54 +0000 UTC
    </div>
</div>

