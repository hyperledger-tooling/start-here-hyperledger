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
                PR <a href="https://github.com/hyperledger/bevel/pull/2442" class=".btn">#2442</a>
            </td>
            <td>
                <b>
                    update spell and grammer lint workflow
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
        Created At 2023-12-04 13:42:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2441" class=".btn">#2441</a>
            </td>
            <td>
                <b>
                    Rename the Shared charts as per Bevel conventions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Rename storageclass chart
- Rename vault-mgmt chart
- Rename imageautomation chart
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 12:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2440" class=".btn">#2440</a>
            </td>
            <td>
                <b>
                    doc redesign
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
        Created At 2023-12-04 11:56:57 +0000 UTC
    </div>
</div>

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

