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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2299" class=".btn">#2299</a>
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
2. Add _helpers.tpl files for all charts
3. Update the values.yaml files
4. Update the version in chart.yaml files

Modifications in  
platforms/hyperledger-besu/charts platforms/hyperledger-besu/charts/besu-connector
platforms/hyperledger-besu/charts/generate_ambassador_certs platforms/hyperledger-besu/charts/node_besu
platforms/hyperledger-besu/charts/node_key_mgmt
platforms/hyperledger-besu/charts/node_orion
platforms/hyperledger-besu/charts/node_tessera
platforms/hyperledger-besu/charts/node_validator
platforms/hyperledger-besu/charts/orion_key_mgmt
platforms/hyperledger-besu/charts/tessera_key_mgmt

Fixes #2287 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 12:33:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2298" class=".btn">#2298</a>
            </td>
            <td>
                <b>
                    [chore] Latest from main
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
        Created At 2023-06-15 15:54:50 +0000 UTC
    </div>
</div>

