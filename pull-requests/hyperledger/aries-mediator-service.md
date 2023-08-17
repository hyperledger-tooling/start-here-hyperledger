---
layout: default
title: aries-mediator-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mediator-service
---

# aries-mediator-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mediator-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    feature:: Firebase push notification plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows mediator users to configure the mediator to send push notifications via firebase when forwarding messages.

Key features:

- Did-comm protocol for receiving device tokens.
- Saving a token per connection_id.
- Subscribes to forwarding event on event bus.
- Generates auth tokens with firebase service and send notifications via http.
- Configurations for the notification message and max send rate.
- Openapi to get tokens and send notifications via swagger
- Upgraded the aca-py version to 0.9.0. The old version 0.8.0 had issue with loading plugins.

Notes:
- Currently there is no unit tests (todo)
- While I know poetry is preferred over pip I was having a lot of trouble getting it to working with the plugin. Can address this later but this was working.
- Currently the sensitive service account json is being loaded as an env variable. This should perhaps be changed to read a file in the directory and force users of it to load the file in their CI/CD pipeline.

TODO: 

- Currently the plugin data store never removes connection <-> token rows when connections are removed. I thought of doing a daemon type service to check the connection table and removing orphaned rows in the token table. Another approach would be to add a connection removed event onto the event bus and then subscribe to it in the plugin. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 23:44:14 +0000 UTC
    </div>
</div>

