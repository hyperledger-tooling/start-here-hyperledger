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
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    Bugfix: timeout error crashing explorer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## This PR:
- resolves `discoveryError` not resetting `waitingResp` flag, causing a `Have already been sending a request` loop.
```
[WARN] FabricGateway - Failed to send discovery request for channel Error: DiscoveryService has failed to return results
    at DiscoveryService.send (.../blockchain-explorer/node_modules/fabric-common/lib/DiscoveryService.js:370:10)
    at processTicksAndRejections (internal/process/task_queues.js:97:5)
...
[INFO] FabricGateway - Have already been sending a request
[INFO] FabricGateway - Have already been sending a request
[INFO] FabricGateway - Have already been sending a request
[INFO] FabricGateway - Have already been sending a request
[INFO] FabricGateway - Have already been sending a request
```
- resolves `queryChainInfo` timeout error killing explorer.
```
[ERROR] Sync - <<<<<<<<<<<<<<<<<<<<<<<<<< Synchronizer Error >>>>>>>>>>>>>>>>>>>>>
[ERROR] Sync - FabricError: Query failed. Errors: ["Error: REQUEST TIMEOUT"]
    at SingleQueryHandler.evaluate (.../blockchain-explorer/node_modules/fabric-network/lib/impl/query/singlequeryhandler.js:47:23)
    at processTicksAndRejections (internal/process/task_queues.js:97:5)
    at async Transaction.evaluate (.../blockchain-explorer/node_modules/fabric-network/lib/transaction.js:276:25)
[INFO] Sync - <<<<<<<<<<<<<<<<<<<<<<<<<< Closing client processor >>>>>>>>>>>>>>>>>>>>>
[DEBUG] FabricEvent - disconnectEventHubs()
[DEBUG] FabricEvent - disconnectChannelEventHub(defaultchannel)
``` 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-27 07:08:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    BE-857 Change invoking function of lifecycle scc to get CC info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change allows non-admin client credential to bring up Explorer instance. And also updated fabric-network package to v2.2.7

Signed-off-by: Atsushi Neki <nekiaiken@gmail.com>

https://jira.hyperledger.org/browse/BE-857
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-26 12:26:02 +0000 UTC
    </div>
</div>

