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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/563" class=".btn">#563</a>
            </td>
            <td>
                <b>
                    lamejs optional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                see https://github.com/hyperledger-labs/business-partner-agent/pull/552
and https://github.com/antoine92190/vue-advanced-chat/issues/190

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/563"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-02 07:24:45 +0000 UTC
    </div>
</div>

