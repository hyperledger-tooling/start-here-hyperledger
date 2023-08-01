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
                PR <a href="https://github.com/hyperledger/bevel/pull/2329" class=".btn">#2329</a>
            </td>
            <td>
                <b>
                    [ci-skip] enable prometheus for besu node metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(besu): enable prometheus for besu node metrics 

prometheus server deployments for individual organizations

fixes #2290
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 09:47:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2324" class=".btn">#2324</a>
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
platforms/r3-corda-ent/charts/auth
platforms/r3-corda-ent/charts/bridge
platforms/r3-corda-ent/charts/float
platforms/r3-corda-ent/charts/gateway
platforms/r3-corda-ent/charts/generate-pki-node
platforms/r3-corda-ent/charts/generate-pki
platforms/r3-corda-ent/charts/h2
platforms/r3-corda-ent/charts/idman
platforms/r3-corda-ent/charts/nmap
platforms/r3-corda-ent/charts/node-initial-registration 
platforms/r3-corda-ent/charts/node
platforms/r3-corda-ent/charts/notary-initial-registration 
platforms/r3-corda-ent/charts/notary
platforms/r3-corda-ent/charts/signer
platforms/r3-corda-ent/charts/zone

Fixes #2284
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 09:15:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2322" class=".btn">#2322</a>
            </td>
            <td>
                <b>
                    [ci-skip]Fix operations console and remove legacy code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following fixes:
- Update for fabric-operations-console
- vault-auth and vault-reviewer creation removed from fabric (only shared role to be used)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 11:40:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2321" class=".btn">#2321</a>
            </td>
            <td>
                <b>
                    [ci-skip] add README.md files for each Helm chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**docs(fabric): add README.md files for each Fabric Helm chart**

```
This commit adds the README.md file for each Fabric Helm chart. The README.md files provide essential information and instructions about the respective Helm charts, enabling users and developers to deploy each chart individually.

Additionally, the following changes have been made:

 • Updated values.yaml of each Helm chart with default values to provide a clear configuration reference.
 • Added helpers.tpl template file only to Helm charts where it was missing, ensuring consistency across the charts.
 • Updated the description and version fields of each Fabric Helm chart.

These changes enhance the usability and documentation of the Fabric Helm charts, making it easier for users and developers to understand and work with the charts.
```

fixes #2283
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 10:03:00 +0000 UTC
    </div>
</div>

