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
                    Bevel Release 0.13.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.13.0.0
                </span>
            </td>
            <td>
                ## What's new in Bevel
- QBFT consensus option added on HL Besu network deployment

## New Features
- HL Fabric
  - Upgrade running Hyperledger Fabric 1.4.x deployment to Hyperledger Fabric 2.2.x deployment
  - Added monitoring for fabric peer and orderer
## Deprecation
  - No active support for older versions of platforms. Check [compatibility matrix](https://blockchain-automation-framework.readthedocs.io/en/latest/compatibilitymatrix.html)
## Major Bug Fixes
  -  flux uninstall issue in reset-network.yaml #2077
  -  duplicate generation of private, public keys even if they are present in vault #2090
  -  docs vault paths fixed #2140 
  -  fixed incorrect image names in supplychain examples app #2138
  -  fixed vault auth issue when Kubernetes node restart #2074 
  -  skip ambassador installation when already installed #2128  

## Known issue

- Intermittent flux installation/uninstallation issues #2157 
- Pods crashes post Kubernetes cluster nodes are restarted #2155 

## Improvements
- Besu
    - Refactor charts to removing dependency on external tools and artifacts
    - Separate crypto generation and genesis file creation
    - Added ability to pass chain Id
    - Separate the process of crypto-generation and joining network when adding a new org/node
    - Added Kubernetes labels to components
    - Added Besu supplychain express app build and push workflow
- Shared
    - Upgraded helm chart for HAProxy

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v0.13.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-03-02 10:58:14 +0000 UTC
    </span>
</div>

