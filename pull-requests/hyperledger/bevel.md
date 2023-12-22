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
                PR <a href="https://github.com/hyperledger/bevel/pull/2460" class=".btn">#2460</a>
            </td>
            <td>
                <b>
                    [fabric] init required in the chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------

1. Support init required option for chaincode approval and commit operation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-22 06:06:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2459" class=".btn">#2459</a>
            </td>
            <td>
                <b>
                    [fabric] Chaincode commit not working
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1.Fixed error in the commit chaincode and invoke chaincode jobs because the organization name contains a '-' 
2.Fixed conflict of the variable orderer.address in platforms/hyperledger-fabric/configuration/roles/k8_component/templates/existing_peer_cli.tpl that caused errors in fabric operations or in deployment of the external chaincode

Modifications
-----------------------
platforms/hyperledger-fabric/charts/fabric-chaincode-commit/templates/commit_chaincode.yaml 
platforms/hyperledger-fabric/charts/fabric-chaincode-invoke/templates/invoke_chaincode.yaml 
platforms/hyperledger-fabric/configuration/roles/k8_component/templates/existing_peer_cli.tpl

fixes #2451
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 13:36:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2458" class=".btn">#2458</a>
            </td>
            <td>
                <b>
                    [shared] update bevel-vault.sh script for sh shell compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## **Commit to be reviewed**


```
feat(shared): update bevel-vault.sh script for sh shell compatibility

Change:
- Modified bevel-vault.sh script for sh shell compatibility.

fixes #quick-fix
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 13:33:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2455" class=".btn">#2455</a>
            </td>
            <td>
                <b>
                    updated repo readme platform overview images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Update overview images
- Added substrate overview 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 10:20:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2452" class=".btn">#2452</a>
            </td>
            <td>
                <b>
                    [fabric] Update adding a new channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1.Update adding a new channel playbook to be compatible with version 2.5.4 2.Fixed the bug with elimination of ServiceAccount and ClusterRoleBinding

Modifications
-----------------------
docs/source/archive/certificates/fabric.md
platforms/hyperledger-fabric/charts/fabric-osnadmin-channel-create 
platforms/hyperledger-fabric/configuration/add-new-channel.yaml 
platforms/hyperledger-fabric/configuration/roles/create/channel_artifacts 
platforms/hyperledger-fabric/configuration/roles/create/genesis 
platforms/hyperledger-fabric/configuration/roles/create/new_orderer 
platforms/hyperledger-fabric/configuration/roles/create/new_organization/orderer_org/syschannel 
platforms/hyperledger-fabric/configuration/roles/create/orderers 
platforms/hyperledger-fabric/configuration/roles/create/osnchannels 
platforms/hyperledger-fabric/configuration/roles/create/refresh_certs/create_channel_block 
platforms/hyperledger-fabric/configuration/roles/delete/vault_secrets 
platforms/hyperledger-fabric/configuration/roles/upgrade/application-capabilities
platforms/hyperledger-fabric/configuration/roles/upgrade/orderer-binary 
platforms/hyperledger-fabric/configuration/roles/upgrade/orderer-capabilities platforms/shared/configuration/roles/create/shared_helm_component/templates/vault_kubernetes_job.tpl

fixes #2439 #2443
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 07:34:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2450" class=".btn">#2450</a>
            </td>
            <td>
                <b>
                    hotfix: quorum tessera fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- quorum tessera container now uses bash 
- storage class chart name change
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 14:35:30 +0000 UTC
    </div>
</div>

