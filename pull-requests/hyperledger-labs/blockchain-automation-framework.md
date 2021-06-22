---
layout: default
title: blockchain-automation-framework
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-automation-framework
---

# blockchain-automation-framework <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-automation-framework){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1539" class=".btn">#1539</a>
            </td>
            <td>
                <b>
                    docs: add angelaalagbe as a contributor for doc, content
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add @angelaalagbe as a contributor for doc, content.

This was requested by sownak [in this comment](https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1535#issuecomment-865861288)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 10:23:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1535" class=".btn">#1535</a>
            </td>
            <td>
                <b>
                    [shared] Edits made to docs so far
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angela Alagbe <angela.alagbe@accenture.com>

**Changelog**
- Added extra lines when needed to create new lines
- Fixed an image formatting issue and a table error
- Updated punctuation and grammar

 

**Reviewed by**
@suvajit-sarkar @sownak 

 

**Linked issue**
#1512 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 11:56:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1534" class=".btn">#1534</a>
            </td>
            <td>
                <b>
                    [quorum] Implemented test for create/constellation rol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add new test for create/constellation rol
- Fixed task using notest tag or changed_when: false to be able to run the implemented test


**Reviewed by**
@suvajit-sarkar
@alvaropicazo

 

**Linked issue**
#725 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 10:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1533" class=".btn">#1533</a>
            </td>
            <td>
                <b>
                    [quorum] fixed molecule test errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Fixed quorum crypto-ibft molecule test errors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 19:54:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1532" class=".btn">#1532</a>
            </td>
            <td>
                <b>
                    [indy] fix docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Update versions for software in docs
- Fix empty cacert file
- Update default ambassador ports

 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 16:27:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1531" class=".btn">#1531</a>
            </td>
            <td>
                <b>
                    [besu] create orion crypto using helmcharts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add orion_crypto helmchart
- Fix orion binary problem
- Update ansible to use orion-job to create orion crypto
- Remove -bes from folder structure


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 10:02:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1530" class=".btn">#1530</a>
            </td>
            <td>
                <b>
                    [besu] Adding a new validator organization with multiple nodes to existing network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Added validator-new-org network.yaml sample
- Fixed what was causing the restart of the existing validator nodes (their value files were being updated and that is not supposed to happen).
- Updated validator_node role for supporting the addition of a new validator node in an existing org to an existing network and the addition of a new validator org with one or multiple validator nodes.

 

**Reviewed by**
@suvajit-sarkar 
@jagpreetsinghsasan 
@sownak 

 

**Linked issue**
#1017

*Screenshots*

![all-validators](https://user-images.githubusercontent.com/76157062/122366131-91cc7000-cf5b-11eb-91a3-12c8c863e70f.PNG)

After the add-validator playbook finished, a new validator org was added (ssalv-bes) containing two validator nodes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 09:03:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1529" class=".btn">#1529</a>
            </td>
            <td>
                <b>
                    [quorum] changed namespace in my converge and prepare, edited verify in parall…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …el with these changes

Signed-off-by: Angela Alagbe <angela.alagbe@accenture.com>

**Changelog**
- Add idempotence notest to nested main
- Fixed bug
- Updated verify.yaml

 

**Reviewed by**
@suvajit-sarkar 

 

**Linked issue**
#1527 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 08:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1528" class=".btn">#1528</a>
            </td>
            <td>
                <b>
                    [shared] cleanup share versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- add default versions on shared roles and cleanup playbooks for:
    - **setup/kubectl** :  default in defaults/main.yaml to 1.16.3, can be override from playbook
    - **setup/helm**   default in defaults/main.yaml to v3.2.4, can be override from playbook
    - **setup/vault** default in defaults/main.yaml to v1.7.0, can be override from playbook
    - **setup/aws-auth** default in defaults/main.yaml to v1.10.3, can be override from playbook
    - **setup/ambassador** version is locked in helm chart


**Reviewed by**
@sownak , @suvajit-sarkar 

 

**Linked issue**
#1511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 06:48:56 +0000 UTC
    </div>
</div>

