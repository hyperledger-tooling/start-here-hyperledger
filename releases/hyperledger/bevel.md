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
                    Bevel Release 1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0.0
                </span>
            </td>
            <td>
                ## What's new in Bevel
- Documentation redesigned and restructured
- Support for Fabric v2.5 network deployment and operations
- Network deployment and operations using GitHub actions workflow 
- Standalone helm charts

## New Features
- HL Besu
  - Deployment using just Bevel Besu helm charts
  - Deployment without hashicorp vault
- HL Fabric 
  - External chaincode deployment on version v2.5
  - Chaincode upgrade/update for external chaincode
 
## Deprecation
- No active support for older versions of Bevel (below v0.15.0)
- Raft and Ethash consensus support removed from Besu
- Support on Kubernetes below v1.23
- Support for lets encrypt for tls cert creation
  
## Known issues
- Corda-ent deployment using firewall 
## Major Bug Fixes
- bug(share) ServiceAccount and ClusterRoleBinding are removed on second run #2443

## Improvements
- Spell and Grammar linting workflow
- bevel-vault script updated for shell compatibility
- indy-key-mgmt. script update to prevent injections

## Documentation
- Playbook and role inline comments
- Helm chart Readme
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v1.0.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-01-23 10:09:17 +0000 UTC
    </span>
</div>

