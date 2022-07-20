---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    Added Event Publication to Relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Implemented 2 endpoints in `EventPublish`, to handle event data from driver and remote-relay.
2. Added an endpoint to fetch all received states: `GetEventStates` and protobuf message for output.
3. Added sdk function for above endpoint, and sample command for it in fabric-cli.
4. Added sample command in fabric-cli to start express server to listen to events.
5. Added more status to `RequestState`, also added status `DELETED` for cleanup of db states in relay (not implemented yet, TODO).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 17:05:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/295" class=".btn">#295</a>
            </td>
            <td>
                <b>
                    Transaction Listener Support in Fabric Driver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added logic to the Fabric driver to start block or chaincode event listeners upon an event subscription request.
Minor upgrades, bug fixes, CLI augmentation, and documentation enhancements.
Fixes #269 and #270 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 21:45:12 +0000 UTC
    </div>
</div>

