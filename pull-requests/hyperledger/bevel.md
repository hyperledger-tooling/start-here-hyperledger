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
                PR <a href="https://github.com/hyperledger/bevel/pull/2244" class=".btn">#2244</a>
            </td>
            <td>
                <b>
                    [substrate] Updated persona
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
        Created At 2023-05-15 16:53:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2241" class=".btn">#2241</a>
            </td>
            <td>
                <b>
                    [besu] refactor crypto creation and genesis tasks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change-log**

- Move crypto create task to k8s jobs
- Refactor genesis creation tasks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 13:56:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2240" class=".btn">#2240</a>
            </td>
            <td>
                <b>
                    [substrate] Add support for Substrate based DSCP platform
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes the following changes
- New platform `substrate` is introduced
- Used `dscp-node` as the substrate node template which will be used in examples as well
- Adds image automation for flux with flux version upgrade
- Fixes formatting errors in docs so Maintainers are listed in readthedocs
- A sample github actions file to deploy a DLT network with Bevel on GCP
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 13:42:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2239" class=".btn">#2239</a>
            </td>
            <td>
                <b>
                    [besu] Decopule Vault CURD Operations in helm charts 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes:

Vault CURD operations have been decoupled and are moved to a script where the vault Script will be created as a configmap in each organizational namespace and will be mounted as a volume in helm charts.

Reviewers:
  @suvajit-sarkar @jagpreetsinghsasan @sownak 

Issues:
#2221 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 12:31:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2238" class=".btn">#2238</a>
            </td>
            <td>
                <b>
                    [ci-skip]: add 'none' as a new option for transaction manager.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---
feat(quorum): add 'none' as a new option for transaction manager.

```
Updated the following files to introduce the new option for transaction manager:
  1. deployment.yaml file of chart node_quorum_member
  2. memberquorum.tpl template
  3. deploy-network.yaml file
  4. network-schema.json
  5. sample network-quorum.yaml file
  6. sample network-quorum-constellation.yaml
```

fixes #2234
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 12:09:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2236" class=".btn">#2236</a>
            </td>
            <td>
                <b>
                    [besu] Add extradata field in genesis file QBFT consensus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Added extradata field in genesis file. platforms/hyperledger-besu/configuration/roles/create/genesis/qbft role
2. Added templates to create genesis file

Modifications in roles and tpl files
-----------------------
platforms/hyperledger-besu/configuration/roles/create/genesis/qbft/tasks/main.yaml 
platforms/hyperledger-besu/configuration/roles/create/genesis/qbft/templates/qbftGenesisFile.tpl platforms/hyperledger-besu/configuration/roles/create/genesis/qbft/templates/qbftPermissionGenesisFile.tpl

Fixes
#2233 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 12:46:45 +0000 UTC
    </div>
</div>

