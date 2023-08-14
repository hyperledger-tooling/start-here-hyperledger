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
                PR <a href="https://github.com/hyperledger/bevel/pull/2345" class=".btn">#2345</a>
            </td>
            <td>
                <b>
                    [fabric] Added creation of Vault auths through cluster_id.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Added creation of Vault auths through cluster_id.
2. Fixed errors related to storage class for the add orderer operation

Modifications in roles and tpl files
-----------------------
platforms/hyperledger-fabric/configuration/add-orderer.yaml platforms/hyperledger-fabric/configuration/deploy-network.yaml platforms/hyperledger-fabric/configuration/roles/create/anchorpeer/tasks/nested_anchorpeer.yaml 
platforms/hyperledger-fabric/configuration/roles/create/ca_tools/orderer/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/channels/tasks/valuefile.yaml 
platforms/hyperledger-fabric/configuration/roles/create/channels_join/tasks/nested_channel_join.yaml 
platforms/hyperledger-fabric/configuration/roles/create/new_orderer/create_appchannel_block/tasks/nested_create_cli.yaml platforms/hyperledger-fabric/configuration/roles/create/new_orderer/create_syschannel_block/tasks/nested_create_cli.yaml platforms/hyperledger-fabric/configuration/roles/delete/vault_secrets/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/anchorpeer_job.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/approve_chaincode_job.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/ca-orderer.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/ca-peer.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/ca-tools.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/cacerts_job.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/cli.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/commit_chaincode_job.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/create_channel_job.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/install_chaincode_job.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/install_external_chaincode_job.tpl platforms/hyperledger-fabric/configuration/roles/helm_component/templates/instantiate_chaincode_job.tpl platforms/hyperledger-fabric/configuration/roles/helm_component/templates/invoke_chaincode_job.tpl platforms/hyperledger-fabric/configuration/roles/helm_component/templates/join_channel_job.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/orderernode.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/upgrade_chaincode_job.tpl platforms/hyperledger-fabric/configuration/roles/helm_component/templates/value_peer.tpl 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/vault_kubernetes_job.tpl 
platforms/hyperledger-fabric/configuration/roles/k8_component/templates/existing_peer_cli.tpl 
platforms/hyperledger-fabric/configuration/roles/k8_component/templates/orderer_cli.tpl 
platforms/network-schema.json
platforms/shared/charts/vault-k8s-mgmt/templates/job.yaml

Fixes
#1847 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 11:26:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2344" class=".btn">#2344</a>
            </td>
            <td>
                <b>
                    [fabric] move hashicorp vault functions to a single script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**

**feat(fabric): move hashicorp vault functions to a single script**

```
This commit decouples the vault related functionality from individual helm charts by utilizing the bevel-vault.sh script.

Changes made:

 • Removed vault-related code from individual Fabric Helm charts.
 • Updated all Helm charts to utilize the shared bevel-vault.sh script.
 • Deleted the vault_kubernetes_job.tpl template file from Fabric platform as we already move this feature to the shared platform.
 • Deleted the verify_chaincode Helm chart from Fabric platform as it is not in use and also there is no .tpl template file for the same Helm chart.

These changes will improve code maintainability and efficiency by reducing code duplication and making it easier to maintain consistency.
```

fixes #2323
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 10:23:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2342" class=".btn">#2342</a>
            </td>
            <td>
                <b>
                    feat(besu): added support for azure storageclass for Hyperledger Besu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 18:01:22 +0000 UTC
    </div>
</div>

