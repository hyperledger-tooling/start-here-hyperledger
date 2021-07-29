---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/561" class=".btn">#561</a>
            </td>
            <td>
                <b>
                    Activity/Task - query from view
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add new events and listeners separate from Aries Events.
Will use new event listeners to notify frontend via sockets (will create new message structure for frontend notifications if needed).

After talking with the team, we are now persisting the activities/tasks. It is populated through events fired from managers. Currently tracking - connection events and presentation exchange events.

Will use the same event listener to fire messages to the frontend which can be used to show badges to users that something new has happened. Show the badges in the most suitable location.

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/561"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 04:45:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/560" class=".btn">#560</a>
            </td>
            <td>
                <b>
                    Webhook Security
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With version 0.5.6 or 0.6 added the possibility to add a secret to the webhook flag. With this feature it is possible to also enable security on the webhook endpoint in the backend.  

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/560"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 15:26:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/559" class=".btn">#559</a>
            </td>
            <td>
                <b>
                    Set partner name in backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See: https://github.com/hyperledger-labs/business-partner-agent/issues/546

UI probably needs more cleaning up. 

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/559"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 10:47:10 +0000 UTC
    </div>
</div>

