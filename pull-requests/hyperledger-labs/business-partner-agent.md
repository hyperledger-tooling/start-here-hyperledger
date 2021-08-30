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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/589" class=".btn">#589</a>
            </td>
            <td>
                <b>
                    attempt to fix action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Action to publish docs currently fails because of DCO

Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/589"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 11:39:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/588" class=".btn">#588</a>
            </td>
            <td>
                <b>
                    add links to clips and add screenshot to readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/588"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 11:11:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/585" class=".btn">#585</a>
            </td>
            <td>
                <b>
                    Feature/receive invite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the Add Partner page to allow connect by DID and connect by Invitation Url.

This is to support connecting with non-phone Agents (ex. Trinsic Studio) that are only generating QR Codes and invitations. This allows us to take their generated invitation and create a Partner.

Currently tested and connected using our own invitations (connection and out of band) and an Invitation from Trinisic Studio.

I have added a simple single redirect handler when reading the invitation url. This is for implementations like Trinsic Studio, where they generate a short url (and thus a simpler easier to read qr code) that will take you to the real underlying invitation url (trinisic uses `d_m` query param, but results in a connection 1.0 invitation).

**Query Params for invitations**

- `c_i` (Aries RFC 0160: Connection Protocol)
- `d_m` (RFC 0268: Unified DIDCOMM Deeplinking)
- `oob` (Aries RFC 0434: Out-of-Band Protocol 1.1)




<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/585"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 02:18:05 +0000 UTC
    </div>
</div>

