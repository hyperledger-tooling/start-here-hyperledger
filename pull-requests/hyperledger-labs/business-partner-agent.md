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
                    Activity/Task - persistence and events from backend to frontend notifications.
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

Hooked the backend notification events to the frontend, and set the indicator badges to read these new stores. Added the `new-message-icon` onto Partner presentations to see which one was recently updated.

We will have to pay attention to which events we want to populate which badge/icon, some events may not make sense, but we can deal with that in a future PR.

Messages will be refactored in a future PR, as we will add persistence, which will change the event/notification model and how the `chat-window` is populated.

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/561"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 04:45:41 +0000 UTC
    </div>
</div>

