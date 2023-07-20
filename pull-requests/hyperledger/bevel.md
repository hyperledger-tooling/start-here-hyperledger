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
                PR <a href="https://github.com/hyperledger/bevel/pull/2320" class=".btn">#2320</a>
            </td>
            <td>
                <b>
                    [ci-skip] Merge main to develop
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
        Created At 2023-07-20 09:49:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2319" class=".btn">#2319</a>
            </td>
            <td>
                <b>
                    [docs] change to git_access_token
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
        Created At 2023-07-20 08:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2318" class=".btn">#2318</a>
            </td>
            <td>
                <b>
                    [ci-skip] Fix binary download and error in vault management chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">besu</span>
            </td>
            <td>
                Fixes besu issues
- rename organizationItem to org as in many shared roles org is used
- Add besu binary download which was removed accidentally when genesis creation was modified
- Update `platforms/shared/configuration/roles/setup/vault_kubernetes` role as it was removing vault-auth on repeat deployments
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 14:14:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2317" class=".btn">#2317</a>
            </td>
            <td>
                <b>
                    [ci-skip] Add README.md files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
Add readme files for all charts
Update the values.yaml files
Update the version in chart.yaml file

Modifications in charts
---------------------
platforms/r3-corda/charts/doorman-tls
platforms/r3-corda/charts/doorman
platforms/r3-corda/charts/generate-certs
platforms/r3-corda/charts/h2
platforms/r3-corda/charts/mongodb-tls
platforms/r3-corda/charts/mongodb
platforms/r3-corda/charts/nms-tls
platforms/r3-corda/charts/nms
platforms/r3-corda/charts/node-initial-registration 
platforms/r3-corda/charts/node
platforms/r3-corda/charts/notary-initial-registration 
platforms/r3-corda/charts/notary

Fixes #2285
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 10:09:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2315" class=".btn">#2315</a>
            </td>
            <td>
                <b>
                    [ci-skip] simplify Storage Class generation with a common Helm Chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(shared): simplify Storage Class generation with a Shared Helm Chart**

```
Simplifies the process of generating storage classes by utilizing a shared Helm chart. The four platforms that have been modified to make them compatible with the shared "storage_class" Helm Chart are:
 • Hyperledger-Fabric
 • R3-corda-Ent
 • Hyperledger-Besu
 • Quorum

The following changes have been implemented:
 • Updated variables to align with the shared Helm chart.
 • Introduced common variables to streamline the configuration of storage classes across different platforms.
 • Updated the HR file responsible for configuring the shared "storage_class" Helm chart.

These changes will simplify the generation of various storage classes by utilizing a single template file. Additionally, they will improve compatibility with the shared "storage_class" Helm chart across multiple platforms.
```

fixes #2306
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 10:16:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2314" class=".btn">#2314</a>
            </td>
            <td>
                <b>
                    [besu] use default securityContext
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
This commit implements the following changes:
- use the securityContext in the besu and validator nodes.

These changes enable besu and validator nodes to run with default securityContext.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 15:10:35 +0000 UTC
    </div>
</div>

