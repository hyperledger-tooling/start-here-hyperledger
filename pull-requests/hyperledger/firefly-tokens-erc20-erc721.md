---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    Use separate eventstream per namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is designed to be compatible with changes in FireFly Core in this PR https://github.com/hyperledger/firefly/pull/1388

Overview of changes:

- The token connector does not automatically create event streams on startup anymore
- When a websocket client connects, it must now send a `start` command for a specific namespace like FireFly Core
- When a namespace is started, the connector will create a websocket connection to the blockchain connector and set up or reuse the existing token event stream for that namespace
- Multiple clients can listen on the same namespace
- Websocket messages will be randomized across all listening clients for a namespace
- When one client disconnects from a namespace, all in-flight messages for that namesake will be nack'd back to the blockchain connector
- If all clients for a given namespace disconnect, the token connector will disconnect its websocket to the blockchain connector
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 18:19:30 +0000 UTC
    </div>
</div>

