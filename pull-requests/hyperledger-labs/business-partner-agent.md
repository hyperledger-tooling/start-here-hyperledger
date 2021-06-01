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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/442" class=".btn">#442</a>
            </td>
            <td>
                <b>
                    Delete values.schema copy.json
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
        Created At 2021-05-30 09:04:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    fix schema
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
        Created At 2021-05-30 09:03:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/440" class=".btn">#440</a>
            </td>
            <td>
                <b>
                    add json schema for some helm values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow to use forms for helm deployments

Signed-off-by: Frank Bernhardt <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-30 06:28:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    Merge pull request #1 from hyperledger-labs/master
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update to origin master
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-30 04:31:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/437" class=".btn">#437</a>
            </td>
            <td>
                <b>
                    fix helm semantic versioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                latest version was not correctly semantic versioned

Signed-off-by: Frank Bernhardt <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 20:32:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    Refresh partners on new partner event and small fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - refresh partners on new partner event.
- Fix in partnerUtils.
- Layout of NewMessageIcon

Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 14:22:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/434" class=".btn">#434</a>
            </td>
            <td>
                <b>
                    Refactor Helm Charts add support for Keycloak and Schemas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Infrastructure</span><span class="chip">frontend</span>
            </td>
            <td>
                Refactored the helm charts.

I have moved `bpa.schemas` into it's own file, and that will have to be loaded via `-Dmicronaut.config.files=classpath:application.yml,classpath:schemas.yml`. But this allows us to create a ConfigMap that contains only schema information (as yaml) that can be loaded via helm charts (mounted as a volume). Adding schemas to runtime is controlled with the values file: `schemas.enabled=true`.

`application.yml` and `security-keycloak.yml` can be configured with ENV VARS, so the ConfigMaps for application and keycloak are Name/Value pairs and those ConfigMaps are loaded as env vars.  `security-keycloak.yml` is optional and controlled with the values file: `keycloak.enabled=true`.

Added in new templates for creating Openshift routes. These are optional and must be enabled and ingresses disabled. Was having lots of issues getting secured routes created using the ingress templates, this seemed easier.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 02:24:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    fix value
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
        Created At 2021-05-26 16:21:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    fix given seed behaviour
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
        Created At 2021-05-26 15:46:05 +0000 UTC
    </div>
</div>

