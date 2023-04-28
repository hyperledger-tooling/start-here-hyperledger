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
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    feat(shared): updated repo and chart path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **updated repo and chart path in the new bevel-samples repository for following platforms**

  1. Besu
  2. Corda
  3. Fabric
  4. Quorum

fixes #2222
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 11:24:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    [chore] merge from main
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
2. updated restserver

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
        Created At 2023-04-26 06:02:34 +0000 UTC
    </div>
</div>

