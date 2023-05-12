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
  1. deployment.yaml file of chart node_quorum_member.
  2. memberquorum.tpl template.
  3. deploy-network.yaml file.
  4. network-schema.json.
  5. sample network-quorum.yaml file.

In addition, added a label to the job.yaml files of the following charts:
  1. certs-ambassador-quorum.
  2. crypto_ibft.
  3. crypto_raft.
  4. tessera_key_mgmt.
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

