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

Currently, this supports Create protocol (`c_i`) urls. We will be supporting Out Of Band (`oob`) urls as soon as https://github.com/hyperledger-labs/acapy-java-client/commit/a1a6b3019959246e39e99862fc48328d73f97039 is added to our code. This will be different PR.

I have added a simple single redirect handler when reading the invitation url. This is for implementations like Trinsic Studio, where they generate a short url (and thus a simpler easier to read qr code) that will take you to the real underlying invitation url (trinisic uses `d_m` query param, but results in a connection 1.0 invitation).

**Query Params for invitations**

- `c_i` (Aries RFC 0160: Connection Protocol)
- `d_m` (RFC 0268: Unified DIDCOMM Deeplinking)
- `oob` (Aries RFC 0434: Out-of-Band Protocol 1.1)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 02:18:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/584" class=".btn">#584</a>
            </td>
            <td>
                <b>
                    Presentation Requests with Proof Templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Send proof templates instead of schemas via presentation requests
- Adapt UI flow and proof template component

![image](https://user-images.githubusercontent.com/87176157/130406842-4affe8c9-b548-4bd9-af23-128be71364b6.png)
![image](https://user-images.githubusercontent.com/87176157/130406898-50925f2d-e95e-4106-bd8f-9e1fca68ca96.png)


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/584"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 07:23:19 +0000 UTC
    </div>
</div>

