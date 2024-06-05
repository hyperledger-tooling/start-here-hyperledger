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
                PR <a href="https://github.com/hyperledger/bevel/pull/2574" class=".btn">#2574</a>
            </td>
            <td>
                <b>
                    [indy] enable platform deployment via ansible server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---
**feat(indy): enable platform deployment via ansible-server**

```
This commit introduces support for deploying a decentralized ledger technology (DLT) network using Ansible automation. The changes include:

1. Updated the Ansible codebase to support network deployment in respect of the standalone Helm chart.
2. The following Ansible roles have been introduced to appropriately deploy the network:
   - 1. Generate keys for each node of each organization.
   - 2. Fetch generated keys in JSON format to deploy genesis with known nodes only.
   - 3. Utilize keys stored in the JSON file to configure the genesis with known nodes and then install the genesis block.
   - 4. A secondary genesis setup is also included to support deployment in multiple namespaces for a multi-organization Indy network.
   - 5. Deploy stewards for all organizations.
   - 6. Deploy the endorser.
3. Updated the Reset Ansible code to delete each node's key from the vault, along with the organization policy and Authentication engine.
4. Added an individual role to clean all the network-supported local files (JSON files).
5. Updated the sample network configuration file to provide information on which networks can be deployed using this file and how to customize the network by following the network rules specified in the file itself.
```

fixes #2557
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 07:35:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2573" class=".btn">#2573</a>
            </td>
            <td>
                <b>
                    [fabric] Fix Chart versions and add-cli via helm chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Chart version update in dependencies
- `add-cli` readme updated with helm install option
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-03 13:10:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2572" class=".btn">#2572</a>
            </td>
            <td>
                <b>
                    [fabric] Fix approve chaincode
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
        Created At 2024-05-31 09:32:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2571" class=".btn">#2571</a>
            </td>
            <td>
                <b>
                    [fabric] Helm chart updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Final Helm chart updates for Fabric
- Simplified Fabric network deployment with only helm charts
- HAProxy Ingress upgrade to 0.14.x version to support `ingressClassName`
- Readme simplification
- Sample values updated
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 12:02:41 +0000 UTC
    </div>
</div>

