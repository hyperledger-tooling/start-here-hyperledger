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
                PR <a href="https://github.com/hyperledger/bevel/pull/2515" class=".btn">#2515</a>
            </td>
            <td>
                <b>
                    feat(fabric): Fabric deployment without channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Primary Changes**

1. The roles related to channel have been removed from the site.yaml file.
2. The create/configtx, create/channel_artifacts and create/genesis" roles aren't executed by version 2.5.4.
3. Channel creation can be done afterwards by running the add-new-channel.yaml playbook.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 15:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2512" class=".btn">#2512</a>
            </td>
            <td>
                <b>
                    [quorum] introduce helm chart deployment capability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(quorum): introduce helm chart deployment capability**

```
This commit enhances the deployment process for the Quorum Distributed Ledger Technology (DLT) network by exclusively leveraging Helm charts.

Four new Helm charts have been introduced to streamline the deployment process:
1. quorum-genesis: Initializes the network with specific requirements.
2. quorum-node: Starts the network and allows adding new nodes.
3. quorum-tessera-node: Facilitates privacy by enabling transaction encryption using Tessera.
4. quorum-tlscert-gen: Enables secure access to the node via HTTPS.

Each chart comes with a README to help users customize the network.

These changes make deploying and managing the Quorum DLT network smoother with Helm.

Other Improvements:
1. Added error handling to ensure clean uninstallation of the besu-genesis and besu-tlscert-gen charts.
2. Updated the README's API Call section.
```

fixes #2484
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 09:50:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2511" class=".btn">#2511</a>
            </td>
            <td>
                <b>
                    chore: Updated kubeconfig configuration in storage class helm chart
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
        Created At 2024-02-19 09:09:16 +0000 UTC
    </div>
</div>

