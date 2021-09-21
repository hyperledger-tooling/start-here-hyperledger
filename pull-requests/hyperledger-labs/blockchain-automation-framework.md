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

