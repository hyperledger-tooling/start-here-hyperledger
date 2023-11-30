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
                PR <a href="https://github.com/hyperledger/bevel/pull/2436" class=".btn">#2436</a>
            </td>
            <td>
                <b>
                    [fabric] Support upgrade chaincode for the external chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1.Support upgrade/update chaincode operation for the external chaincode

Modifications
-----------------------
docs/source/operations/upgrading_chaincode.md
platforms/hyperledger-fabric/configuration/external-chaincode-ops.yaml 
platforms/hyperledger-fabric/configuration/roles/create/chaincode/install_ext/tasks/nested_main.yaml 
platforms/hyperledger-fabric/configuration/roles/create/chaincode/peer_certs/tasks/generate_certs.yaml 
platforms/hyperledger-fabric/configuration/roles/create/external_chaincode_server/tasks/valuefile.yaml 
platforms/hyperledger-fabric/configuration/roles/create/peers/tasks/main.yaml 
platforms/hyperledger-fabric/configuration/samples/network-fabricv2-external-chaincode.yaml platforms/network-schema.json

fixes #2352
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 14:40:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2435" class=".btn">#2435</a>
            </td>
            <td>
                <b>
                    feat(shared): Implement GitHub Spellcheck and grammar linting for Pull request.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request implements the GitHub Spellcheck feature to automatically check the spelling and grammar in commit messages for all Pull Requests (PRs).

Changes Made:
- Modified the code to check the grammar errors at exact line numbers. 
- In docs/README.md file corrected the grammar errors.

Fixes: hyperledger#2327
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 07:44:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2434" class=".btn">#2434</a>
            </td>
            <td>
                <b>
                    bug(besu): fix issue with orgs using different vault server
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
        Created At 2023-11-28 04:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2433" class=".btn">#2433</a>
            </td>
            <td>
                <b>
                    [r3-corda-ent] upgrade to version 4.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
---
### feat(r3-corda-ent): upgrade to version 4.10

**Changes:**

- `Node` and `Notary` nodes have been upgraded to version 4.10 (specifically, version 4.10.3) from 4.7.
- Introduced a new Dockerfile, named `node4.10.dockerfile`, to build the version 4.10 image.
- Updated the codebase to fetch the latest version 4.10 properly when the user defines it in the network configuration file.

**Additional changes:**
- Added the missing vault delete commands.
- Fixed the code to delete the vault policy correctly.
- Updated sample network configuration files to facilitate smooth deployment.

---

fixes #2398
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 13:44:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2432" class=".btn">#2432</a>
            </td>
            <td>
                <b>
                    [shared] updated gke csi provisioner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 04:36:06 +0000 UTC
    </div>
</div>

