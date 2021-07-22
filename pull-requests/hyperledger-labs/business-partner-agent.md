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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/557" class=".btn">#557</a>
            </td>
            <td>
                <b>
                    Remove docker-compose-backend-webonly.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Is anybody relying on this?

Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/557"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 10:08:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    Issue 553 - Trusted Issuers aren't stored correctly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #553

Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/556"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 09:58:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    Fix example did's
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/555"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 09:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    Basic Messaging - no persistence.  
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Send message to partner, partner gets event and surfaces to Vuex store.
This illustrates the basic messaging between multiple agents. Each room is for a single partner and your partner.  Messages are not persisted, only stored in VUEX.

This is slightly temporary, as we are going to refine the socket events and messages and notifications. Improvements on this component should include indicating which partner/room has a new message to read. Perhaps we can change this to only show the single partner when we navigate to the business partner detail screen? Another improvement is to keep the list of rooms (partners) in sync with the known partners; currently it will add a partner/room if you are the receiver of a connection.  This should be improved along with the changes to notifications/tasks/activities etc.


Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/552"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 23:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/550" class=".btn">#550</a>
            </td>
            <td>
                <b>
                    Issue: 548 Optional Trustping
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/550"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 17:36:12 +0000 UTC
    </div>
</div>

