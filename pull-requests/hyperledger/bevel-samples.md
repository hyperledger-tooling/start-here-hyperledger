---
layout: default
title: bevel-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel-samples
---

# bevel-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    [fabric] Upgrade Fabric restserver to latest stable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. updated image name for expressapi
2. updated flux namespace in tpl files
2. updated restserver dependencies

Modifications in roles and tpl files
-----------------------
 examples/supplychain-app/configuration/roles/create/fabric/expressapi/tasks/main.yaml
 examples/supplychain-app/configuration/roles/helm_component/templates/expressapi-besu.tpl
 examples/supplychain-app/configuration/roles/helm_component/templates/expressapi-fabric.tpl
 examples/supplychain-app/configuration/roles/helm_component/templates/expressapi-quorum.tpl
 examples/supplychain-app/configuration/roles/helm_component/templates/expressapi.tpl
 examples/supplychain-app/configuration/roles/helm_component/templates/frontend.tpl
 examples/supplychain-app/configuration/roles/helm_component/templates/restserver.tpl
 examples/supplychain-app/configuration/roles/helm_component/templates/webserver.tpl

Modifications for the reserver
-------------------------
 examples/supplychain-app/fabric/chaincode_rest_server/rest-server/Dockerfile
 examples/supplychain-app/fabric/chaincode_rest_server/rest-server/package.json
 examples/supplychain-app/fabric/chaincode_rest_server/rest-server/tsconfig.json
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 12:56:05 +0000 UTC
    </div>
</div>

