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
                PR <a href="https://github.com/hyperledger/bevel/pull/2208" class=".btn">#2208</a>
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
                **Change log**

Update Contribution.md by adding create local branch & directory structure section

Fixes #2131 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 17:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2207" class=".btn">#2207</a>
            </td>
            <td>
                <b>
                    [ci-skip] move common delete network roles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 **Change log**
  Move common delete roles to shared folder
  Update shared playbook names
  Update site.yaml with better indentation
  Refactor logic to delete flux resources
  Docker username validation fix, add "-" in regex

Fixes: #2157 #2206 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 11:02:36 +0000 UTC
    </div>
</div>

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

