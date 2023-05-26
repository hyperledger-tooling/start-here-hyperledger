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
                PR <a href="https://github.com/hyperledger/bevel/pull/2263" class=".btn">#2263</a>
            </td>
            <td>
                <b>
                    [besu] improve error handling mechanism for vault api calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

feat(besu): improve error handling mechanism for vault api calls

```
This pull request introduces improvements to the error handling mechanism and enhances troubleshooting capabilities in the bevel-vault.sh script. The changes made include:
 • Implemented error handling at the individual function level.
 • Enhanced error message logging for better visibility into failures.
 • Improved error checking and validation.
 • Updated paths in respect of the function calls to reflect the latest changes.
```

fixes #2260
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 11:51:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2262" class=".btn">#2262</a>
            </td>
            <td>
                <b>
                    [substrate] Update chart readme's
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added readme and updated Chart.yaml so that the helm charts can be made available as a repo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 11:47:31 +0000 UTC
    </div>
</div>

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
platforms/hyperledger-besu/configuration/roles/create/crypto/node/tasks/main.yaml
platforms/hyperledger-besu/configuration/roles/create/genesis/templates/ibftGenesisFile.tpl
platforms/hyperledger-besu/configuration/roles/create/validator_node/Readme.md
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/check_vault.yaml
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/main.yaml
platforms/hyperledger-besu/configuration/roles/create/validator_node/tasks/validator_vote.yaml

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 11:00:08 +0000 UTC
    </div>
</div>

