---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2155" class=".btn">#2155</a>
            </td>
            <td>
                <b>
                    build(openapi): upgrade openapi-generator version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Commit to be reviewed
------------------------------------

build(openapi): upgrade openapi-generator version   


    Primary Changes
    ---------------
    1. Updated openapitools.json file   
    
    Secondary Changes
    ----------------
    1. Some of the generated kotlin files are updated with the new code

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 06:29:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2154" class=".btn">#2154</a>
            </td>
            <td>
                <b>
                    feat(cbdc-bridging-app): refactor ODAP plugin implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * From now there is one PluginOdapGateway that must be extended by any implementation of a gateway
* This commit intends to decouple the gateway implementation from any ledger
* There is still a Gateway implementation for Fabric and Besu
* The asset being transferred is now in the scope of the request and not the gateway, which makes possible the transfer of multiple assets without having to create new gateways

closes #2132 

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 16:06:35 +0000 UTC
    </div>
</div>

