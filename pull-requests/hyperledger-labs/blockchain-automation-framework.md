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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1555" class=".btn">#1555</a>
            </td>
            <td>
                <b>
                    [besu][quorum] Vault validation function improvement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add improved validation function for vault response in besu: node_orion and node_validator. In quorum: node_tessera and node_constellation

**Tested Scenarios**
Quorum tessera/constellation vault sealed
<img width="688" alt="NetworkQuorum-DeletePod-VaultSealed-tesseraError" src="https://user-images.githubusercontent.com/83813093/124425194-843f2480-dd68-11eb-8f3b-be670b78ac23.png">
<img width="652" alt="NetworkQuorum-DeletePod-VaultSealed-constellationError" src="https://user-images.githubusercontent.com/83813093/124425238-94570400-dd68-11eb-8667-c7f8f3f36dd2.png">

Quorum tessera/constellation vault port changed
<img width="752" alt="NetworkQuorum-DeletePod-VaultPortChanged-tesseraError" src="https://user-images.githubusercontent.com/83813093/124425345-b3ee2c80-dd68-11eb-9b3e-3f916e97d8b7.png">
<img width="754" alt="NetworkQuorum-DeletePod-VaultPortChanged-constellationError" src="https://user-images.githubusercontent.com/83813093/124425366-b9e40d80-dd68-11eb-8776-8aee93a51069.png">

Besu orion/validator vault sealed
<img width="643" alt="NetworkBesu-DeletePod-VaultSealed-memberError" src="https://user-images.githubusercontent.com/83813093/124425564-09c2d480-dd69-11eb-9026-24b2e0126624.png">
<img width="680" alt="NetworkBesu-DeletePod-VaultSealed-validatorError" src="https://user-images.githubusercontent.com/83813093/124425690-2fe87480-dd69-11eb-8108-037187d724bd.png">

Besu orion/validator vault port changed
<img width="694" alt="NetworkBesu-DeletePod-VaultPortChanged-memberError" src="https://user-images.githubusercontent.com/83813093/124425780-57d7d800-dd69-11eb-8a60-3e15807ee0b7.png">
<img width="691" alt="NetworkBesu-DeletePod-VaultPortChanged-validatorError" src="https://user-images.githubusercontent.com/83813093/124425798-5d352280-dd69-11eb-9d12-addda333d30e.png">



**Reviewed by**
@suvajit-sarkar
@alvaropicazo

 
**Linked issue**
#1364 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-05 06:19:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1554" class=".btn">#1554</a>
            </td>
            <td>
                <b>
                    [docs] updated links and matrix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

Updated compatiblity matrix
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 10:01:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1553" class=".btn">#1553</a>
            </td>
            <td>
                <b>
                    [shared] update kubectl to 1.19.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: pppazos <pppazos@gmail.com>

**Changelog**
- upgrade kubectl 1.19.8

 

**Reviewed by**
@sownak @suvajit-sarkar 

 

**Linked issue**
#1538 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 09:51:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1552" class=".btn">#1552</a>
            </td>
            <td>
                <b>
                    [docs] updated roadmap and compatibility table
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Update roadmap and compatibility table

 

**Linked issue**
#1513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 07:50:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1544" class=".btn">#1544</a>
            </td>
            <td>
                <b>
                    [corda-ent] Add new notary org
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add support in corda-enterprise to add new notary
- Fix certificate issues for API and Web
- Update certificate namespaces for OS Corda

 **Linked issue**
Resolves #1414 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 12:11:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1542" class=".btn">#1542</a>
            </td>
            <td>
                <b>
                    [chore] Release merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR to merge develop into master for the current release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 14:32:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1541" class=".btn">#1541</a>
            </td>
            <td>
                <b>
                    [quorum] quorum and tessera version upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Update version for quorum and tessera
- Tessera version 21.4.0 and Quorum 21.4.2
 

**Linked issue**
#1451 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 06:44:52 +0000 UTC
    </div>
</div>

