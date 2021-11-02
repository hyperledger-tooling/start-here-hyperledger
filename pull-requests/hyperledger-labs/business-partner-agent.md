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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/663" class=".btn">#663</a>
            </td>
            <td>
                <b>
                    Feature list in readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added detailed feature list to the readme and updated main description

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/663"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 10:27:53 +0000 UTC
    </div>
</div>

