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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1673" class=".btn">#1673</a>
            </td>
            <td>
                <b>
                    [fabric] Access policies from the configmaps and deployment frabic to vaultv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add configmap in charts /vault_kubernetes
- Fix create/crypto/orderer  and create/crypto/peer (add a new condition in task Get all ambassador secrets from Vault) 
- Fix create/genesis in main.yaml change vault write for vault kv put in task "Create genesis block"
- Fix value_per.tpl and install_chaincode_job.tpl change metadata for data in vault paths
- Update vault_kubernetes_job and ca_server_job to vaultv2


 

**Reviewed by**
@alvaropicazo 
@suvajit-sarkar 


 

**Linked issue**
#1657 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 09:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1672" class=".btn">#1672</a>
            </td>
            <td>
                <b>
                    [quorum] fixed quorum keystore password issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 17:25:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1671" class=".btn">#1671</a>
            </td>
            <td>
                <b>
                    [fabric] updated to support operations console
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add helmchart for Fabric operations console
- Rename ca-server to more appropriate generate_cacerts
- Add support for grpcws for peer and orderer charts
- Add support for Operations API (non TLS) for ca, peer and orderer charts
- Add playbook to deploy operations console and generate json files

 
**Linked issue**
Resolves #1610 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 15:53:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1663" class=".btn">#1663</a>
            </td>
            <td>
                <b>
                    [corda-ent] Updated platform r3 corda-ent roles README.md files.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
 Updated platform r3 corda-ent roles README.md files.

 

@sownak @suvajit-sarkar 

 
1624

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 07:04:06 +0000 UTC
    </div>
</div>

