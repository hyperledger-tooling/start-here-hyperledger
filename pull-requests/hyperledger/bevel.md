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
                PR <a href="https://github.com/hyperledger/bevel/pull/2561" class=".btn">#2561</a>
            </td>
            <td>
                <b>
                    [substrate] enable platform deployment via ansible server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(substrate): enable platform deployment via ansible server**

```
This commit introduces support for deploying a decentralized ledger technology (DLT) network using Ansible automation. The changes include:

- Added a new network configuration file to define nodes (Bootnode, Validator, Member, IPFS) within a single organization.
- Updated the `deployment-network.yaml` to support the new network configuration.
- Updated multiple Ansible roles, Helm release templates, and charts to align with the new network configuration.
- Updated the user guide documentation to assist users/developers in correctly configuring the network.
```

**fixes #2547**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 11:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2560" class=".btn">#2560</a>
            </td>
            <td>
                <b>
                    [fabric] Create channel using just helm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Primary Changes**

1.Deploy fabric 2.5.4 with channel using helm charts. 
2.Deploy fabric 2.2.2 with channel using helm charts. 
3.Delete platforms/hyperledger-fabric/charts/fabric-anchorpper 
4.Deploy with Ansible is pending
5.Update README.md files is pending

**Changes in charts**
platforms/hyperledger-fabric/charts/fabric-ca-server 
platforms/hyperledger-fabric/charts/fabric-catools 
platforms/hyperledger-fabric/charts/fabric-cli
platforms/hyperledger-fabric/charts/fabric-orderernode 
platforms/hyperledger-fabric/charts/fabric-peernode 
platforms/hyperledger-fabric/charts/fabric-channel-join 
platforms/hyperledger-fabric/charts/fabric-channel-create 
platforms/hyperledger-fabric/charts/fabric-osnadmin-channel-create

fixes #2539 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 15:44:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2559" class=".btn">#2559</a>
            </td>
            <td>
                <b>
                    feat(r3-corda-ent): helm only deployment using proxy and vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change log**
- Added code to enable deployment using vault(hashicorp) and proxy (ambassador)
Fixes #2540 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 09:16:53 +0000 UTC
    </div>
</div>

