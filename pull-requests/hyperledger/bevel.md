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
                PR <a href="https://github.com/hyperledger/bevel/pull/2261" class=".btn">#2261</a>
            </td>
            <td>
                <b>
                    chore(docs): fix discord link
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
        Created At 2023-05-25 13:30:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2254" class=".btn">#2254</a>
            </td>
            <td>
                <b>
                    [besu] Decouple crypto creation for Besu operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Added generation of cryptography through a job for besu operations
2. Fixed syntax error in tpl file for generation of genesis for ibft consensus

Modifications in roles
-----------------------
platforms/hyperledger-besu/configuration/add-validator.yaml
platforms/hyperledger-besu/configuration/roles/create/genesis/templates/ibftGenesisFile.tpl 
platforms/hyperledger-besu/configuration/roles/create/validator_node/Readme.md 
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/add_to_vault.yaml 
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/check_vault.yaml 
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/create_enode.yaml 
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/main.yaml 
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/validator_vote.yaml
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 11:00:08 +0000 UTC
    </div>
</div>

