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
                    Bevel Release 0.12.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.12.0.0
                </span>
            </td>
            <td>
                ## What's new in Bevel
- Upgraded to use flux-v2.
- Added support to for deployment on Kubernetes v1.20+
- Added operation to refresh certificate in HL Fabric platform
- Support for Corda OS node v4.9

## New Features
- HL Fabric
  - Operation to attach CLI to already running peer node
  - Enable multiple chaincodes installation on peer
## Deprecation
  - No active support for older versions of platforms. Check [compatibility matrix](https://blockchain-automation-framework.readthedocs.io/en/latest/compatibilitymatrix.html)
## Major Bug Fixes
  -  Adding a new organization in Hyperledger Fabric operation fails #1932 
  -  fabric: wrong EtcdRaft.Consenters.Port generated in configtxOrderer_default.tpl and configtxProfile_default.tpl #1907 
  -  docs(quorum): update the readme bugs #1886 
  -  Install chaincode doesn't fail when invalid git details are provided #1952 
  -  Cannot find schema '/network-schema.json' #1929

## Version Upgrades
- Deployment Environment
  - Python 3.8
  - Ansible [core 2.12.6]
  - Openshift 0.13.1

## Improvements
- Shared
    - Updated bevel-build docker images with version changes
    - DCI lint tool for inclusive language checks for PR
- All platforms
   - ImagePullPolicy changed to IfNotPresent
- Quorum
  - Ansible decoupling raft crypto creation
- HL Fabric
  -  Updated the hyperledger-fabric platform sample configuration files
  -  Logic added to fail pod on vault access issues/missing credential 
- Documentation
  - Updated docs with version change
  - Update/added troubleshooting guide links
  - Update inclusive language changes
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v0.12.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-11 10:54:07 +0000 UTC
    </span>
</div>

