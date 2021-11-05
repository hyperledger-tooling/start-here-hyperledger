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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/668" class=".btn">#668</a>
            </td>
            <td>
                <b>
                    Get rid of remaining auto flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is about fixing some remaining issues in the exchange states.

1. Store credential information on credential issued (issuer) and credential received (holder) events, as the acked event is only a courtesy and might not be implemented by all agents.
2. Disable auto respond credential request flag. This one is a bit tricky as in v1 indy a credential request event is always preceeded by an offer, so here we can always auto respond because the user has already accepted the offer. Whereas in v2 a holder can initiate the flow directly. This means running an agent with this auto flag enabled results in auto issuance, which could be a security issue when running none test bpa instances. So I changed the behaviour in the v2 handler that credential requests without a prior offer are denied. We can implement this flow later for v2, which is a nice shortcut feature.
3. Disable auto store credential on the holder side. 



Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/668"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 13:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    fixing holder revocation states in partner details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/667"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 09:54:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/666" class=".btn">#666</a>
            </td>
            <td>
                <b>
                    Bug: get Cred Ex for review was triggering state change
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When the issuer wants to review the credential exchange (what we issued and whether it was accepted/declined), we just need the data from the db. Was calling the full check to see if it is in db and wallet (important for holder), this was triggering a state change to problem once the credentials exchange is auto-removed from the wallet - so this little fix ensures we can read historical data stored in BPA db. However, the original call that compares db and wallet is important (particularly for the holder) as the conversation/exchange is ongoing. 

Not sure what is going on with my local docker, but it was NOT picking up the changes to acapy images, so my local dev was using a slightly older version and this wasn't an issue.  🤷 

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/666"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 17:30:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/665" class=".btn">#665</a>
            </td>
            <td>
                <b>
                    Lts alpine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Need to keep the node image at 14, using its-alpine just jumped up to 16 and there were sass generation issues.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/665"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 19:45:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/664" class=".btn">#664</a>
            </td>
            <td>
                <b>
                    Update notification badges logic for manual vs auto Cred Exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #662 

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/664"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-30 00:15:55 +0000 UTC
    </div>
</div>

