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
                    BAF beta release 0.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.9.0.0
                </span>
            </td>
            <td>
                ## What's new in BAF
- BAF R3 Corda Enterprise and Corda OS node version 4.7 deployment support
- BAF R3 Corda Enterprise CENM version 1.5 deployment support
- Added and updated baf-build image for java 8 and java 14

## New Features
- Shared
  - Complete support and option to use Flux and Git either over SSH or HTTPs 
- HL Besu:
  - Updated HL Besu and Orion version support
  - Added Tessera support
- HL Indy 
  - Version update
- HL Fabric:
  - Expose CA server via HAProxy
  - Add the anchor peer support for the addition of new peer in fabric
  - Add new organization to the consortium
  - Addition of annotations for pods/components supplied via network.yaml

## Deprecation
- No active support for older versions of platforms.

## Major Bug Fixes
- Join channel and Anchor Peer update tasks resulted in failure for a configuration with multiple channels in HL Fabric network #1392 
- Adding new org should add to existing channel and consortium #1297
- Unable to remove an org from the live channel after the org has gone unreachable in HL Fabric Network - DR Scenario #1408 

List of all bug fixes can be found [here](https://github.com/hyperledger-labs/blockchain-automation-framework/issues?q=is%3Aissue+label%3A%22Release+0.9.0.0%22+label%3Abug)

## Improvements 
- Molecule Test
  - Added more testing scenarios for platforms code 
  - Added platforms molecule tests in Git Actions for PR checks
- R3 Corda Enterprise
  - Improve validation function for vault responses
- Share
  - Updated Ambassador version to 1.11.0 and platform code to use v2 annotations
  - Separate namespace for flux (non default)
  - Create ambassador tls secret in organization namespace 
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/releases/tag/v0.9.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-06-30 16:43:42 +0000 UTC
    </span>
</div>

