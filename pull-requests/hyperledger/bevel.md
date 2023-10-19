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
                PR <a href="https://github.com/hyperledger/bevel/pull/2394" class=".btn">#2394</a>
            </td>
            <td>
                <b>
                    feat(shared): add missing files for OS-specific command handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Quick fix commit to be reviewed**
---

**feat(shared): add missing files for OS-specific command handling**

```
Description:
- In the PR titled "feat(shared): enable OS-specific command handling in Helm charts," I forgot to include certain files.
- I thought that changing the name of the Helm chart would override the updated file only, not the entire chart, but I was wrong.
- This PR will address the missing file and fulfill the purpose of the original PR.
```

fixes #quick-fix
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 12:18:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2393" class=".btn">#2393</a>
            </td>
            <td>
                <b>
                    bug(r3-corda-ent): delete HashiCorp vault access and policies on network reset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
This pull request addresses the need to delete HashiCorp Vault access and policies when performing a network reset.

changes made in:
1. platforms/r3-corda-ent/configuration/cleanup.yaml
2. platforms/r3-corda-ent/configuration/roles/delete/vault_secrets/tasks/main.yaml

fixes:#2390
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 05:03:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2392" class=".btn">#2392</a>
            </td>
            <td>
                <b>
                    [fabric] Update chaincode charts to be compatible with version 2.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
 1. Updated  chaincode charts
 2. Fixed a bug that occurred when creating the genesis file with an incorrect channel name

Modifications in docs
-----------------------
docs/source/_static/TopLevelClass-Fabric.png
docs/source/operations/fabric_networkyaml.md

Modifications in charts
-----------------------
platforms/hyperledger-fabric/charts/commit_chaincode/templates/commit_chaincode.yaml platforms/hyperledger-fabric/charts/install_chaincode/templates/install_chaincode.yaml

Modifications in roles and tpl files
-----------------------
platforms/hyperledger-fabric/configuration/chaincode-ops.yaml platforms/hyperledger-fabric/configuration/deploy-network.yaml platforms/hyperledger-fabric/configuration/roles/helm_component/templates/commit_chaincode_job.tpl

Others Modifications
----------------------------------------
platforms/hyperledger-fabric/configuration/samples/network-fabricv2.yaml

fixes #2385
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 10:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2389" class=".btn">#2389</a>
            </td>
            <td>
                <b>
                    fix:(corda-ent, shared) chart liniting errors, aes host ns hardcoding
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
        Created At 2023-10-17 06:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2388" class=".btn">#2388</a>
            </td>
            <td>
                <b>
                    [shared] enable OS-specific command handling in helm charts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---
**feat(shared): enable OS-specific command handling in helm charts**

```
This PR improves the handling of OS-specific commands within Helm charts.

Changes:
- Introduced a script to check the Operating System and its supporting package manager for efficient package installation.
- Added a ConfigMap object to insert the same above-mentioned script into the container, improving flexibility and compatibility.

Additional change:
- Updated the StorageClass Helm chart to resolve the node affinity issue.

There are only 3 platforms that are currently using OS-Specific Command in Helm Charts directly, and this PR is also made for these 3 platforms only:
- Quorum
- Hyperledger-Fabric
- Substrate
```

fixes #2366
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 05:49:17 +0000 UTC
    </div>
</div>

