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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1566" class=".btn">#1566</a>
            </td>
            <td>
                <b>
                    [besu] Update to vault v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Fix besu binary download links
- Update vault commands to v2 


**Linked issue**
Resolves #1548 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 11:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1565" class=".btn">#1565</a>
            </td>
            <td>
                <b>
                    [chore] latest merge from develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Latest merge from develop branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 11:22:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1564" class=".btn">#1564</a>
            </td>
            <td>
                <b>
                    [shared] network.yaml schema validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Add network-schema.json with shared and corda schemas
- Add ajv-cli tool to docker image
- Update run.sh script to validate network.yaml file before execution

 

**Reviewed by**
@suvajit-sarkar @sownak 

 

**Linked issue**
#1558 
#1559

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 08:22:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1561" class=".btn">#1561</a>
            </td>
            <td>
                <b>
                    [besu] Vault validation function improvement for tessera and besu nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add improved validation function for vault response in besu: node_tessera and node_besu. 

**Tested Scenarios**
Besu tessera/besu vault sealed
<img width="668" alt="NetworkBesu-DeletePod-VaultSealed-memberError-tessera" src="https://user-images.githubusercontent.com/83813093/124573525-e9b71200-de49-11eb-924e-d4911ace2d17.png">

Besu tessera/besu vault port changed
<img width="716" alt="NetworkBesu-DeletePod-VaultPortChanged-memberError-tessera" src="https://user-images.githubusercontent.com/83813093/124573657-0ce1c180-de4a-11eb-8601-2ac8979e0368.png">

 

**Reviewed by**
@suvajit-sarkar
@alvaropicazo

 

**Linked issue**
#1364 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 09:06:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1560" class=".btn">#1560</a>
            </td>
            <td>
                <b>
                    [shared] updates for k8s 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Remove unused png files
- Update Ingress and rolebinding as per Kubernetes 1.19
- Update Flux version to 1.23.0
- Update HAProxy version to 0.12.5
- Update Ambassador to 1.13.9 
- Update helm to v3.6.2
 

**Linked issue**
Resolves #1538 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 09:00:45 +0000 UTC
    </div>
</div>

