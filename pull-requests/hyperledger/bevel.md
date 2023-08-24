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
                PR <a href="https://github.com/hyperledger/bevel/pull/2351" class=".btn">#2351</a>
            </td>
            <td>
                <b>
                    feat(shared): Simplifying storage class creation with helm module 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request addresses to refactor the current implementation of creating helm releases using GitOps to a more flexible approach by leveraging the ansible helm module and moving the creation of storage class roles to a share folder.

The six platforms that have been modified to make them compatible with the shared "storage class" charts and roles are:
   • Hyperledger-Besu
   • Hyperledger-Fabric
   • R3-corda
   • R3-corda-Ent
   • Quorum
   • Hyperledger- Indy

Changes Made:

Instead of using gitOps to create helm release, used helm module from ansible by creating jinja(j2) template. Moved the creation of storage class roles to a shared folder to use them across all the platforms.

Fixes: #2306
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 15:05:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2347" class=".btn">#2347</a>
            </td>
            <td>
                <b>
                    [fabric] update orderer pods and update required image versions compatible with 2.5.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Primary Changes
--------------
1. Updated port of operations in orderers pods to avoid errors
2. Added fabric 2.5.x compatible versions of images: couchdb and ca_image
3. Removed fabrictools image in generate_cacerts job as it is not being used

Modifications in charts
-----------------------
platforms/hyperledger-fabric/charts/generate_cacerts/values.yaml 
platforms/hyperledger-fabric/charts/orderernode/templates/configmap.yaml 
platforms/hyperledger-fabric/charts/orderernode/templates/deployment.yaml 
platforms/hyperledger-fabric/charts/orderernode/templates/service.yaml

Modifications in roles and tpl files
-----------------------
platforms/hyperledger-fabric/configuration/roles/create/ca_server/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/ca_server/vars/main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/peers/vars/main.yaml 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/cacerts_job.tpl

Fixes
#2346 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 13:00:50 +0000 UTC
    </div>
</div>

