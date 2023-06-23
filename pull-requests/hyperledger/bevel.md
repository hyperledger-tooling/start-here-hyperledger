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
                PR <a href="https://github.com/hyperledger/bevel/pull/2305" class=".btn">#2305</a>
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
1. Add readme files for all charts
2. Update the values.yaml files
3. Update the version in chart.yaml file

Modifications in charts
platforms/r3-corda/charts/doorman-tls
platforms/r3-corda/charts/doorman
platforms/r3-corda/charts/generate-certs
platforms/r3-corda/charts/h2-addUser
platforms/r3-corda/charts/h2-password-change
platforms/r3-corda/charts/h2
platforms/r3-corda/charts/mongodb-tls
platforms/r3-corda/charts/mongodb
platforms/r3-corda/charts/nms-tls
platforms/r3-corda/charts/nms
platforms/r3-corda/charts/node-initial-registration 
platforms/r3-corda/charts/node 
platforms/r3-corda/charts/notary-initial-registration 
platforms/r3-corda/charts/notary platforms/r3-corda/charts/storage

Fixes #2285
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 11:51:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2304" class=".btn">#2304</a>
            </td>
            <td>
                <b>
                    [ci-skip] Added readme's for all the helm charts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs(indy): Added readme's for all the helm charts for platform indy

Add readme files for all charts
Add _helpers.tpl files for all charts
fixes #2288

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 05:37:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2302" class=".btn">#2302</a>
            </td>
            <td>
                <b>
                    [ci-skip] improved descriptions in Chart.yaml files for all Helm charts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(quorum): improved descriptions in Chart.yaml files for Quorum platform Helm charts**

```
- This commit enhances the descriptions in the Chart.yaml files for all Quorum platform Helm charts.
- The updates ensure that the descriptions accurately reflect the functionality and purpose of each Helm chart.

Additionally:
- Fix the Verification section of each README.md's file.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 11:11:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2301" class=".btn">#2301</a>
            </td>
            <td>
                <b>
                    [ci-skip] fix hardcoded port 8443 and introduce the ordererAddress field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---
**feat(fabric): fix hardcoded port 8443 and introduce the ordererAddress field**

```
This commit removes all occurrences of the hardcoded port and introduces a new field called ordererAddress. This new field will be used to refer to the orderer address, similar to how peerAddress is used for the peer address.

Changes Made:
- Removed all occurrences of port 8443 in the Fabric codebase.
- Introduced the new ordererAddress field for referring to the orderer address.

By making this change, it is no longer necessary to rely on a proxy check when determining the orderer or peer address. This improves flexibility and makes the codebase more maintainable.
```

fixes: #2273
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 12:40:34 +0000 UTC
    </div>
</div>

