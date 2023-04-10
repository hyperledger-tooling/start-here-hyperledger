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
                PR <a href="https://github.com/hyperledger/bevel/pull/2204" class=".btn">#2204</a>
            </td>
            <td>
                <b>
                    [ci-skip] reset fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">fabric</span>
            </td>
            <td>
                Changes:
 Updated the reset-network.yaml to have new roles under roles/delete, there new roles would delete  the  cluster roles, clusterrolebindings, patch and delete gitrepositories, patch and delete kustomizations, helm charts, helm releases and the namespaces

         "delete/clusterrole"
         "delete/clusterrolebindings"
         "delete/gitrepositories"
         "delete/kustomization" 
         "delete/helm_charts"
         "delete/helm_releases"
         "delete/organizations_namespaces"
         "delete/flux_namespaces"

Reviewers:
@suvajit-sarkar @sownak @jagpreetsinghsasan 

Fixes:
#2157 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 11:32:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2201" class=".btn">#2201</a>
            </td>
            <td>
                <b>
                    [docs] updated contribution.md with create local branch & directory structure
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
        Created At 2023-04-06 08:17:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2199" class=".btn">#2199</a>
            </td>
            <td>
                <b>
                    [ci-skip] updated reset.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---
bug(quorum): updated reset.yaml
```
Added patching and deletion code for the following kubernetes resources
 1. ClusterRole
 2. ClusterRoleBinding
 3. GitRepository
 4. Kustomization
 5. HelmChart
 6. HelmRelease
 7. Organizations namespaces
 8. flux namespace
```

fixes #2157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 12:23:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2198" class=".btn">#2198</a>
            </td>
            <td>
                <b>
                    [ci-skip] updated reset.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                bug(r3corda): updated reset.yaml
```
Added patching and deletion code for the following kubernetes resources
1. ClusterRole
2. ClusterRoleBinding
3. GitRepository
4. Kustomization
5. HelmChart
6. HelmRelease
7. Organizations namespaces
8. flux namespace
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 08:49:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2197" class=".btn">#2197</a>
            </td>
            <td>
                <b>
                    [besu] add resource checks to reset.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Commit to be reviewed

bug(besu): add resource checks to reset.yaml  

    Added resource checks for the following K8s resources:
     1. Gitrepositories
     2. Kustomizations
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 13:56:22 +0000 UTC
    </div>
</div>

