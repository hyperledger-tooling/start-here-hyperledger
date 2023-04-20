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
                PR <a href="https://github.com/hyperledger/bevel/pull/2216" class=".btn">#2216</a>
            </td>
            <td>
                <b>
                    [ci-skip] Ansible decoupling for create/users
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Updated ca-tools chart
2. Updated ca-tool tpl file
3. Updated platforms/hyperledger-fabric/configuration/roles/create/ca-tools/peer role
4. Deleted platforms/hyperledger-fabric/configuration/roles/create/users role

Modifications in roles and tpl files
-----------------------
platforms/hyperledger-fabric/configuration/roles/create/ca-tools/peer/Readme.md 
platforms/hyperledger-fabric/configuration/roles/create/ca-tools/peer/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/users/Readme.md 
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/ca-tools.tpl

Modifications in charts
-------------------------
platforms/hyperledger-fabric/charts/catools/templates/configmap.yaml 
platforms/hyperledger-fabric/charts/catools/templates/deployment.yaml 
platforms/hyperledger-fabric/charts/catools/values.yaml
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 07:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2215" class=".btn">#2215</a>
            </td>
            <td>
                <b>
                    [chore] Correct spelling
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
        Created At 2023-04-14 17:07:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2214" class=".btn">#2214</a>
            </td>
            <td>
                <b>
                    [chore] : rename shared roles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change log**

- Renamed shared roles from platform/shared/configuration/roles/create/shared_helm_component to helm_component.
- Renamed shared roles from platform/shared/configuration/roles/create/shared_k8s_secrets to k8s_secrets.
- Renamed shared roles from platform/shared/configuration/roles/delete/shared_k8s_secrets to k8s_secrets.

Fixes: https://github.com/hyperledger/bevel/issues/2129
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 13:54:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2211" class=".btn">#2211</a>
            </td>
            <td>
                <b>
                    [ci-skip] add delete for releases with org-namespace folder names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change log**

- add delete for releases with org-namespace folder names
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 11:47:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2210" class=".btn">#2210</a>
            </td>
            <td>
                <b>
                    [docs] update the readme and docs with updated playbook names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change log**
Fix add org playbook with new playbook names
Fix typo in k8s_secret role
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 07:24:16 +0000 UTC
    </div>
</div>

