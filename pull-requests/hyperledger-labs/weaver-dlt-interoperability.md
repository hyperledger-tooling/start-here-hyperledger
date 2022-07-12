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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Weaver Fabric Driver changes for events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes address (pertaining to Fabric Driver):

- Event subscription
- Event unsubscription
- Event listing
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 14:47:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    Relay: Event Subscription Endpoints implemented
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Feature:
1. Event subscription endpoints added in relay.
2. Added new service in protos `relay/events` to make event subscription completely async in relay.
3. Added new fields in `EventMatcher` proto.
5. Bump Relay version and Protos version to 1.4.0.
6. (EDIT) Added event subscription api in fabric-sdk.
7. (EDIT) Added sample command in fabric-cli to register for an event.
8. (EDIT2) Added unsubscription endpoint in relay.
9. (EDIT2) Relay now fetches sign and cert from driver on the subscription request.
10. (EDIT2) Added unsubscribe api in weaver-sdk and sample command in fabric-cli. 
11. (EDIT3) Added get subscription status api in weaver SDK and sample command in fabric-cli.
12. (EDIT3) Updated Subscription Status protos enum.

Improvements:
1. Moved all committed fabric-network artifacts to separate folder, which will be copied to `shared` folder during network start, and deleted when run `make clean`.
2. Added workflow to test relay using dummy driver and dummy client.
3. (EDIT2) Code reorganization in Relay to re-use existing code in different endpoints.
4. (EDIT2) Fixed warnings in Relay compilation.

Close #267 #272 #292 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 17:36:21 +0000 UTC
    </div>
</div>

