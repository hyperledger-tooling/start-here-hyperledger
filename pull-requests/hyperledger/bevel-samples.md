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
                PR <a href="https://github.com/hyperledger/bevel-samples/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    [shared] Add delete roles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Added platforms/shared/configuration/roles/delete roles for deleting realese files and fluxes
2. Added platforms/shared/configuration/delete-app.yaml playbook for execution of delete roles

Modifications in platforms/shared/configuration
-----------------------
platforms/shared/configuration/delete-app.yaml
platforms/shared/configuration/roles/delete/flux/tasks/main.yaml platforms/shared/configuration/roles/delete/flux/tasks/nested.yaml platforms/shared/configuration/roles/delete/gitops/README.md platforms/shared/configuration/roles/delete/gitops/tasks/main.yaml

Fixes
https://github.com/hyperledger/bevel/issues/2237
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 16:01:28 +0000 UTC
    </div>
</div>

