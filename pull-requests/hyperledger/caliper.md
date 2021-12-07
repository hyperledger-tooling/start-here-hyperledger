---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1183" class=".btn">#1183</a>
            </td>
            <td>
                <b>
                    Fix issue where init flow errors when not using mutual TLS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                although init flows should not be used with the new connectors if you do it shouldn't fail but it fails with the following error if you aren't using mutual TLS

TypeError: this.connectorConfiguration.getConnectionProfileDefinitionForOrganization(...).isTLSEnabled is not a function

closes #1160
Signed-off-by: D <d_kelsey@uk.ibm.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 15:48:43 +0000 UTC
    </div>
</div>

