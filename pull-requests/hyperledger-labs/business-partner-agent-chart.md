---
layout: default
title: business-partner-agent-chart
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent-chart
---

# business-partner-agent-chart <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent-chart){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    liveness and readyness now
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: frank-bee <Frank.Bernhardt@bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 12:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent-chart/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Feature/ux config update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes were made to the actual configuration expected by the BPA code.
This updates deal with that (basically remove some properties from the configuration).
The Chart appVersion matches with the build that supports these configuration changes.

I also simplified the ux configuration as @frank-bee previously suggested. It makes it easier to understand when it is all in one place. So there are 3 preset options: `bcgov`, `custom`, `default`.

`default` does nothing, no configmaps, no volumes/mounts, lets the application run with the default ux.
`custom` is used when defining the configuration in your own `values.yaml`
`bcgov` loads the configuration as defined in `bpa_configmap_ux.yaml`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 19:49:28 +0000 UTC
    </div>
</div>

