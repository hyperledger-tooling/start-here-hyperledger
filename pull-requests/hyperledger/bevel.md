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
                PR <a href="https://github.com/hyperledger/bevel/pull/2219" class=".btn">#2219</a>
            </td>
            <td>
                <b>
                    [ci-skip] Fix remove org errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">fabric</span>
            </td>
            <td>
                Fixed following errors
- remove org for Fabric was failing because of latest shared changes, it was removing the flux 
- Update to samples
- Renamed shared files correctly
- Updated Job waiting so that it succeeds even when pods were deleted but jobs were complete
- Update helm uninstall
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 16:36:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2218" class=".btn">#2218</a>
            </td>
            <td>
                <b>
                    [ci-skip] Pods crashes post Kubernetes cluster nodes are restarted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Fixed permission denied error for vault.
2. Fixed vault-auth bug 
3. Fixed removal of vault policies for r3-corda

Modifications in roles and tpl files
-----------------------
platforms/quorum/configuration/roles/create/k8_component/templates/reviewer_rbac.tpl 
platforms/r3-corda-ent/configuration/roles/create/k8_component/templates/reviewer_rbac.tpl 
platforms/r3-corda/configuration/roles/create/k8_component/templates/reviewer_rbac.tpl 
platforms/r3-corda/configuration/roles/delete/vault_secrets/tasks/nested_main.yaml
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 06:48:29 +0000 UTC
    </div>
</div>

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

