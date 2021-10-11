---
layout: default
title: blockchain-automation-framework
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/blockchain-automation-framework
---

# blockchain-automation-framework <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-automation-framework){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    BAF Release 0.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.10.0.0
                </span>
            </td>
            <td>
                ## What's new in BAF
- BAF code upgraded to use Hashi Corp vault secret engine version 2
- BAF code upgraded and tested for EKS version 1.19
- BAF code now validates the network.yaml before deployment
## New Features
- HL Besu:
  - Added deployment option with Ethash and Clique consensus
  - Enabled proxy none option
## Deprecation
  - No active support for older versions of platforms. Check [compatibility matrix](https://blockchain-automation-framework.readthedocs.io/en/latest/compatibilitymatrix.html)
## Major Bug Fixes
  - Shell command - cat not working for huge files during vault write operation #1642
  - List of all bug fixes can be found [here](https://github.com/hyperledger-labs/blockchain-automation-framework/issues?q=is%3Aissue+is%3Aclosed+label%3A%22Release+0.10.0.0%22++label%3A%22bug%22)
## Known Issues
  - Quorum network deployment broken #1703
## Improvements
- Molecule Test
  - More testing scenarios covered for Corda OS and Quorum
- HL Besu
  - Improve validation function for vault responses in helm charts
  - Tessera crypto management via k8s job
  - Separate pods for Besu and Tessera deployment
- Quorum
  - Improve validation function for vault responses in helm charts
  - Tessera crypto management via k8s job
  - Separate pods for quorum and Tessera deployment
  - IBFT crypto management via k8s job
- HL Fabric
  - Vault Kubernetes setup in k8s job
  - CA server certificate creation in k8s job
- Shared 
  - Added baf-build image build in GitHub Actions
  - Added corda image build in GitHub Actions
  - Added Quorum express-app image build in GitHub Action
  - Added Quorum smartcontract static tests in GitHub Action
  - Added chaincode/smartcontract static test in GitHub Action 
  - Updated Ambassador version to 1.13.9
- Documentation
  - Update platform r3 corda OS and enterprise configuration README.md files  
  - Update quorum certificate paths documentation
  - Update the documentation to include the operational features for HL Besu
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/releases/tag/v0.10.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-10-11 10:00:49 +0000 UTC
    </span>
</div>

