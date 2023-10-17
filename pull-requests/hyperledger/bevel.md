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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2387" class=".btn">#2387</a>
            </td>
            <td>
                <b>
                    update(docs): add readthedocs config file
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
        Created At 2023-10-11 18:05:33 +0000 UTC
    </div>
</div>

