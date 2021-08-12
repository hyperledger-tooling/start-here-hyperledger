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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Ux/move did off dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The DID being the first thing users see confuses them as they don't know what it means. 

Moved it to the settings page for us.

New dashboard: 
![image](https://user-images.githubusercontent.com/5376854/129115131-178f63f6-c92a-4cc9-a2ff-a8acd68e70e0.png)

New settings page:
![image](https://user-images.githubusercontent.com/5376854/129115190-8ba6986f-7696-478d-8a04-494cc0e0dbd3.png)


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/570"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 23:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/569" class=".btn">#569</a>
            </td>
            <td>
                <b>
                    Virtual Partner Name/Alias
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently when we add a new Partner the Partners name is always pre filled with the partners legal name (if set). This can cause confusion because like this the partners alias is always set as well. For example:

1. agent 1 adds a new partner with legal name foo
2. partner changes legal name to bar
3. agent 1 reloads partner, legal name changes to bar, display name stays foo

This is totally correct as this adheres to our partner name strategy, but it is very confusing to the user. So instead of using two way binding to set the alias I only set the placeholder like this,

<img width="721" alt="Screen Shot 2021-08-11 at 16 34 47" src="https://user-images.githubusercontent.com/13498217/129050143-c6d76c08-8f05-45dd-9c2c-3ad1452c5c61.png">

then the user can set a real alias if needed.

<img width="696" alt="Screen Shot 2021-08-11 at 16 34 56" src="https://user-images.githubusercontent.com/13498217/129050188-46935d9c-7408-4c0a-945d-2faf40de94cf.png">


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/569"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 14:36:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/567" class=".btn">#567</a>
            </td>
            <td>
                <b>
                    Feature/message persistence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Persist the Aries Basic Messages between partners.
Update the load and fetch mechanism for using the stored messages.
Show indicators beside each partner in the chat that has unread messages.

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/567"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-07 00:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/566" class=".btn">#566</a>
            </td>
            <td>
                <b>
                    Add credential revocation/revocation status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added the possibility to revoke issued credentials in the credential management section and in the partner details.
- Display revocation status of credentials in the verified credentials section within my wallet

Wallet Credential Revocation status

<img width="1525" alt="Screen Shot 2021-08-10 at 15 24 30" src="https://user-images.githubusercontent.com/13498217/128876214-70f1eede-b7a5-4102-97b2-5e1d07068214.png">

Partner Details Revocation Status

<img width="1534" alt="Screen Shot 2021-08-09 at 16 25 34" src="https://user-images.githubusercontent.com/13498217/128722663-c1d1ce98-dce7-4f18-b8c4-73a82468f146.png">

Issue Credential - Revocation Status

<img width="1605" alt="Screen Shot 2021-08-09 at 16 25 17" src="https://user-images.githubusercontent.com/13498217/128722676-5ce26849-417f-48a4-88fd-8b53a30d29d0.png">


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/566"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 12:24:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/565" class=".btn">#565</a>
            </td>
            <td>
                <b>
                    Keycloak vcauthn login
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New class which replaces micronauts default class if keycloak is being used. 

New class is identical except for presentationRequestConfigurationId member and loading of that value into the parameters of the redirect request. 

Requires `micronaut.security.oauth2.clients.keycloak.vcauthn.pres_req_conf_id` to be set to non-null value other application will not start. Is there a safe way to load this with a default. The ideal behaviour is that keycloak would be able to log in in any way but using the exact vc-authn service that handles the VC Verification would not work without the proper value set. 

Looking for input, could possibly configure a more generic query parameter injection. 



<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/565"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 23:36:27 +0000 UTC
    </div>
</div>

