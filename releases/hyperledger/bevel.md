---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Bevel Release 0.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.11.0.0
                </span>
            </td>
            <td>
                ## What's new in Bevel
- Hyperlederlabs Blockchain automation Framework (BAF) is now Hyperledger Bevel
- R3 Corda enterprise platform automation now has `cenm-console` integrated with cenm services.
- `fabric-operations-console` now can be setup using fabric platform automation
- Quorum/Besu Tessera keys storage integrated with HashiCorp Vault
- Addition of an org to an existing Indy consortium
## New Features
- HL Besu:
  - Added Express app for supplychain application API endpoints
  - Tessera and Besu versions upgraded
- HL Fabric
  - Generation of configtx.yaml with custom templates
- R3 Corda Enterprise
  - New cenm services integrated : Auth, Gateway and Zone Service

## Deprecation
  - No active support for older versions of platforms. Check [compatibility matrix](https://blockchain-automation-framework.readthedocs.io/en/latest/compatibilitymatrix.html)
## Major Bug Fixes
  - Handle chaincode package install retries #1784 
  - Vault root token is used to create secrets in Helmchart in Fabric #1730 
  - Remove the use of vault root token in Corda OS containers #1713 
  - Quorum deployment failing for raft consensus #1721 
## Improvements
- All platforms
   - Added crypto storage checks and retries in helm charts
- HL Besu
  - Ansible decoupling of create/certificates/ambassador and vault_kubernetes role
- Quorum
  - Ansible decoupling of setup/vault_kubernetes role
- HL Fabric
  - Added crypto storage checks and retries in helm charts
  - Vault-Kubernetes setup check done in helm charts
  - Orderer/Peer `tls` certificate creation done via helm charts
  - Handle chaincode package install retries
- Documentation
  - Updated name to Hyperledger Bevel
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v0.11.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-14 08:49:34 +0000 UTC
    </span>
</div>

