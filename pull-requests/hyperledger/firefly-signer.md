---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Add wsbackend client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a JSONRPC WebSocket client. It is fairly basic in its features, but gives the ability to create subscriptions and listen for blocks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 20:19:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Ensure SyncRequest never returns nil, even if context is closed 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```go
// In all return paths *including error paths* the RPCResponse is populated
```

... we say it, but then we return `nil` if the context is closed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 18:13:14 +0000 UTC
    </div>
</div>

