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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    added mycila license plugin, enabled check goal, and reformatted all …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …headers

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 11:24:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    #367 Manual connection request - backend part
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 10:42:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    #385 Feature/connect to personal wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backend</span><span class="chip">enhancement</span><span class="chip">frontend</span><span class="chip">help wanted</span>
            </td>
            <td>
                Issue #385.

First feature PR, please let me know if I mis-used anything. 

API method that passes parameters into acapy `create-invitation` endpoint, injecting service_name based on application config. and returns the aca-py response directly `{invitationUrl:"",connectionId:""}`

Frontend method that makes call on click, and uses qrcode.vue component to render QR code on screen.

I'm unsure on the PartnerManager and ConnectionManager relationship, i connected PartnerController directly to ConnectionManager, but this may have been incorrect if you always want it to go through the partnerManager. 

Issues to fix: 
- [x] `mvn -f backend/pom.xml test spotbugs:check pmd:check` fails
- [ ] After aca-py successfully responds to `connections/create-invitation` it raises an event to the BPA, and the [aca-py client model](https://github.com/boschresearch/aries-acapy-clients/blob/main/java/src/main/java/org/hyperledger/aries/api/connection/ConnectionRecord.java) for that eventhander is too strict in that 'theirLabel' is a required field but is not always provided. 
 _this does not stop the invitation from being used and a connection to be established (it overwrites those values later during the actual connection creation)_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 20:37:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    Feature/fix seedhandling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 13:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    fix helm docu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Bernhardt <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 13:38:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    Feature/helm agent secrets newnew
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                another trial to push these commits ;-)
+ @Jsyro 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 11:59:38 +0000 UTC
    </div>
</div>

