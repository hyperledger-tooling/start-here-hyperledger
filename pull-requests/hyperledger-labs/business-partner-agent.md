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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    Add support for OIDC/Keycloak security.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for OAuth2/OpenID/Keycloak security.
This does not change the current implementation.

I could not figure out how to have a fully working backend only solution with Keycloak. I did have an EndSessionEndpoint configured that would get initialized, but would not get called. The DefaultOpenIdClient always intercepts and does an authorizationRedirect, so immediately after the logout, it would log in automatically. The only way I have it work is for the browser to tell Keycloak to terminate the session (this happens after the backend removes the JWT tokens etc by calling `/logout`).

I did not want to add any additional Keycloak specific libraries to VUE or Java.

Important, this is an additional configuration file (`security-keycloak.yml` that gets loaded AFTER the `application.yml`, so when standing up a container, one must specify the configuration files to load and their order:

```
-Dmicronaut.config.files=classpath:application.yml,classpath:security-keycloak.yml
```

Not supplying this runs the application as normal (with only the local user authentication).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 01:30:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    fixed npe, fixed can not connect to none bpa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 15:20:57 +0000 UTC
    </div>
</div>

