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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2448" class=".btn">#2448</a>
            </td>
            <td>
                <b>
                    [chore] Document redesign first pass
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated the docs as per hyperledger template https://github.com/hyperledger-labs/documentation-template
- Review the formatting and content at https://baf.readthedocs.io/en/feature-doc-redesign/
- Some content needs update

Resolves #2158 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 15:05:50 +0000 UTC
    </div>
</div>

