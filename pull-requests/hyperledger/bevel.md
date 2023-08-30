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
                PR <a href="https://github.com/hyperledger/bevel/pull/2360" class=".btn">#2360</a>
            </td>
            <td>
                <b>
                    [besu] onchain permissioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**docs(besu): onchain permissioning**

```
- This commit aims to improve the documentation and enable users to implement Onchain Permissioning within their Besu networks.
- This guide provides step-by-step instructions and highlights the prerequisites for deploying the Besu Onchain Permissioning Network. It also includes a reference to a sample configuration file for easy customization.
```

fixes #2348
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 13:48:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2356" class=".btn">#2356</a>
            </td>
            <td>
                <b>
                    [shared] update ambassador to latest ambassador edge-stack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Note**
Changes currently test and enabled for **Besu platform** only

**Change log**
- Update ambassador to latest **ambassador edge-stack (aes)** version 3.7.2
- Orion TM support removed, as Orion support is available via Tessera TM
- RPC url will no longer support custom ports and will use http port 80 only, this will save some ports 
- RLPX protocol does not work over http port, and by default does not support SNI, will continue to use custom ports
- Removed creation of self signed tls cert for ambassador tls termination, instead use aes create default one
- network.env.ambassadorPorts.ports should be an array or list for besu. AJV needs to be ignored for this till aes is enabled on all platforms. Suggest using portRange meanwhile 
- network.env.namespace changed to network.env.proxy_namespace

**TODO**
- Enable aes for other platforms
- Test aes with cert manager
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 16:56:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2355" class=".btn">#2355</a>
            </td>
            <td>
                <b>
                    [fabric] Changes to support external chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Changes to support TLS external chaincode
- Renamed chaincode containers so that Flux does not give releaseName format errors because of long names
- removed references to hyperledgerlabs docker images
- updated sstorgacelass name
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 15:21:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2354" class=".btn">#2354</a>
            </td>
            <td>
                <b>
                    [fabric] Update configtx.yaml file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
-------------------
1. Updated .tpl files related to creation of the configtx.yaml file with new features of the fabric 2.5 version

Modifications in roles and tpl files
-----------------------
platforms/hyperledger-fabric/configuration/roles/create/configtx/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/configtx/templates/configtxOrderer_default.tpl platforms/hyperledger-fabric/configuration/roles/create/configtx/templates/configtxOrg_default.tpl 
platforms/hyperledger-fabric/configuration/roles/create/configtx/templates/configtxinit_default.tpl

Fixes
#2350 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 12:31:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2353" class=".btn">#2353</a>
            </td>
            <td>
                <b>
                    feat(shared, besu): added support for azure storage class in shared and besu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request adds basic configuration for Azure storage classes in the Shared directory. It also adds a value for "azure-storageclass" in the Besu configuration.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 04:23:12 +0000 UTC
    </div>
</div>

