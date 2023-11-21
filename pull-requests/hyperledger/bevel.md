---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2431" class=".btn">#2431</a>
            </td>
            <td>
                <b>
                    [fabric] Update add_peer and add_orderer to 2.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1.add_peer updated for version 2.5.4
2.add_orderer updated for version 2.5.4

Modifications
-----------------------
platforms/hyperledger-fabric/charts/fabric-orderernode 
platforms/hyperledger-fabric/charts/fabric-osnadmin-channel-create 
platforms/hyperledger-fabric/configuration/add-orderer.yaml 
platforms/hyperledger-fabric/configuration/add-peer.yaml 
platforms/hyperledgerfabric/configuration/roles/create/new_orderer/create_appchannel_block/templates/update_channel_script.tpl 
platforms/hyperledger-fabric/configuration/roles/create/orderers/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/osnchannels/tasks/valuefile.yaml 
platforms/hyperledger-fabric/configuration/roles/create/peers/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/peers/tasks/nested_main.yaml 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/orderernode.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/osn_create_channel_job.tpl

fixes #2430
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 16:42:36 +0000 UTC
    </div>
</div>

