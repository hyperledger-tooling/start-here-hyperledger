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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2248" class=".btn">#2248</a>
            </td>
            <td>
                <b>
                    [ci-skip] kind cluster for test_molecule workflow 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes:

exposed and published ports 8443 and 10080
Removed the lint from provisioner and verifier in molucule.yml 
upgraded the kind image to bsycorp/kind:latest-1.23 from bsycorp/kind:latest-1.19

Note: This PR is just to fix the kind cluster, There are many roles which are being complained by molecule tests which will be fixed in other Issue

Reviewers:
@suvajit-sarkar @sownak @jagpreetsinghsasan 

Issue:
#2125 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 15:59:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2247" class=".btn">#2247</a>
            </td>
            <td>
                <b>
                    [chore] fix flux role
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
        Created At 2023-05-17 10:50:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2246" class=".btn">#2246</a>
            </td>
            <td>
                <b>
                    [ci-skip]: refactor "tessera" role structure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(quorum): refactor "tessera" role structure**

```
Summary:
- Reorganize the Quorum repository's "tessera" role to improve clarity and maintainability. 
- This commit separates the deployment components, namely "tessera", "member nodes", and "validator nodes", into distinct directories. 
- The changes enhance the navigation and update references and configurations accordingly.

Details:
- Create "member_nodes" and "validator_nodes" directories.
- Preserve "tessera" files in the existing tessera directory.
- Move relevant files for "member nodes" into the "member_nodes" directory.
- Move files related to "validator nodes" into the "validator_nodes" directory.
- Update all necessary references and paths in the repository to reflect the new file locations.

```

fixes #2243
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 06:02:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2245" class=".btn">#2245</a>
            </td>
            <td>
                <b>
                    [ci-skip]: fixed the job length.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                bug(fabric): fixed the job length in the network-schema.json

fixes: #2212
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 06:51:10 +0000 UTC
    </div>
</div>

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

