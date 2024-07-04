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
                    Bevel Release 1.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.0
                </span>
            </td>
            <td>
                ## What's new in Bevel
- Platform's with new standalone helm charts, allowing network deployment using just helm commands. 
- Network deployment with proxy or without proxy (single cluster dev/poc setup)
- Network deployment with Hashicorp Vault or without Vault with Kubernetes secrets 

## New Features
- HL Fabric 
  - Network deployment without channel creation
  - Support for custom labels in services and deployments
 
## Deprecation
- No active support for older versions of Bevel (below v1.0.0)
- Support on Kubernetes below v1.23
- No support for Fabric < 2.2.x
  
## Known issues
- Corda Enterprise deployment using firewall support disabled
- 
## Major Bug Fixes
- policy_type variable undefined #2473
- Incorrect storage class name #2513
- RLPx Handshake Error in Quorum Validator Nodes #2563

## Improvements
- All Platform helm charts refactored 
- Hahsicorp Vault paths made flat for easier usage/readability for all platforms

## Documentation
- Update the readme's, setup guide and version information for the DLT platforms
- Update operations guide

## What's Changed
* [fabric] Support add-orderer-organization.yaml playbook by @mgCepeda in https://github.com/hyperledger/bevel/pull/2493
* docs(quorum): operations section under guides tab by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2498
* update(docs): fabric configuration and ops sections by @mgCepeda in https://github.com/hyperledger/bevel/pull/2500
* feat(r3corda): enable DLT deployment via GitHub Workflow & Action. by @sailajakommineni in https://github.com/hyperledger/bevel/pull/2499
* update(docs): Substrate configuration file. by @mgCepeda in https://github.com/hyperledger/bevel/pull/2502
* docs(Hyperleder-besu): operations and configurations section under guides tab by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2503
* [corda] New charts as per release 1.0.0 by @sownak in https://github.com/hyperledger/bevel/pull/2505
* docs(quorum): configuration section under guides tab by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2504
* docs(r3corda): operations section under guide's tab by @sailajakommineni in https://github.com/hyperledger/bevel/pull/2506
* update(docs): Indy configuration and ops sections by @mgCepeda in https://github.com/hyperledger/bevel/pull/2507
* chore: Updated kubeconfig configuration in storage class helm chart by @sownak in https://github.com/hyperledger/bevel/pull/2511
* feat(fabric): Fabric deployment without channel by @mgCepeda in https://github.com/hyperledger/bevel/pull/2515
* feat(besu): implement proposevalidatorvote  method to add or rem… by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2517
* [quorum] introduce helm chart deployment capability by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2512
* [quorum] implement istanbul_propose method to add or remove a node by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2516
* Revert "[quorum] introduce helm chart deployment capability" by @suvajit-sarkar in https://github.com/hyperledger/bevel/pull/2519
* [quorum] introduce helm chart deployment capability by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2520
* [corda] Ansible automation with new helm charts by @sownak in https://github.com/hyperledger/bevel/pull/2521
* doc: update roadmap by @suvajit-sarkar in https://github.com/hyperledger/bevel/pull/2522
* feat(besu): updated  image versions for quorum engineering, besu-node and mysql by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2524
* [chore] Update flux and redis versions by @sownak in https://github.com/hyperledger/bevel/pull/2526
* (fabric): added support for labels in fabric network by @adityajoshi12 in https://github.com/hyperledger/bevel/pull/2528
* [r3-corda] Cordapps download with secrets by @sownak in https://github.com/hyperledger/bevel/pull/2530
* (fabric): syntax fix for annotations by @adityajoshi12 in https://github.com/hyperledger/bevel/pull/2532
* [fabric] Introduce helm chart deployment capability for version 2.5 by @mgCepeda in https://github.com/hyperledger/bevel/pull/2529
* [indy] Upgrade to 1.12.6 and support for Kubernetes 1.28+ by @sownak in https://github.com/hyperledger/bevel/pull/2531
* [substrate] platform deployment via Helm by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2541
* [fabric] Create configtx and genesis files using just helm by @mgCepeda in https://github.com/hyperledger/bevel/pull/2543
* feat(r3-corda-ent) base network deployment using just helm charts by @suvajit-sarkar in https://github.com/hyperledger/bevel/pull/2542
* [fabric] Catools should be dependency of orderer/peer by @mgCepeda in https://github.com/hyperledger/bevel/pull/2552
* [substrate] update helm charts readmes by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2553
* feat(substrate): enable deployment with proxy and vault via helm by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2554
* [indy] Use only helm to deploy Indy network by @sownak in https://github.com/hyperledger/bevel/pull/2555
* feat(r3-corda-ent): helm only deployment using proxy and vault by @suvajit-sarkar in https://github.com/hyperledger/bevel/pull/2559
* [substrate] enable platform deployment via ansible server by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2561
* [fabric] Create channel using just helm by @mgCepeda in https://github.com/hyperledger/bevel/pull/2560
* update(besu,quorum): adapt besu & quorum ansible tasks and template files to charts by @alvaropicazo in https://github.com/hyperledger/bevel/pull/2562
* [fabric] Helm chart updates by @sownak in https://github.com/hyperledger/bevel/pull/2571
* [fabric] Fix Chart versions and add-cli via helm chart by @sownak in https://github.com/hyperledger/bevel/pull/2573
* [fabric] Update add cli and add peer docs by @sownak in https://github.com/hyperledger/bevel/pull/2575
* [fabric] Genesis update and add new channel by @sownak in https://github.com/hyperledger/bevel/pull/2577
* [indy] enable platform deployment via ansible server by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2574
* [shared] support flux latest version 2.3.0 by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2579
* [fabric] Operator readme updates by @sownak in https://github.com/hyperledger/bevel/pull/2580
* [fabric] Update ansible playbooks and roles by @mgCepeda in https://github.com/hyperledger/bevel/pull/2570
* [r3-corda-ent] enable platform deployment via ansible-server by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2582
* [fabric] Update ansible playbooks for create a channel by @mgCepeda in https://github.com/hyperledger/bevel/pull/2589
* shared: hot fix by @mgCepeda in https://github.com/hyperledger/bevel/pull/2592
* chore: merged changes from main to develop by @suvajit-sarkar in https://github.com/hyperledger/bevel/pull/2593
* [docs] Updated for latest release by @sownak in https://github.com/hyperledger/bevel/pull/2595
* [chore] release 1.1 merge by @sownak in https://github.com/hyperledger/bevel/pull/2596


**Full Changelog**: https://github.com/hyperledger/bevel/compare/v1.0.1...v1.1.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v1.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-04 09:14:50 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Bevel Release 1.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.1
                </span>
            </td>
            <td>
                ## What's Changed

**Full Changelog**: https://github.com/hyperledger/bevel/compare/v1.0.0.0...v1.0.1

## What's Changed
* [fabric] Fix approve chaincode by @sownak in https://github.com/hyperledger/bevel/pull/2572
* feat(fabric): update playbooks to refresh certificates for fabric version 2.5.x by @alvaropicazo in https://github.com/hyperledger/bevel/pull/2578
* docs: add repo md files as per lfx best practices by @suvajit-sarkar in https://github.com/hyperledger/bevel/pull/2581
* feat(fabric): update manage-user-certificate playbook to refresh user certificates by @alvaropicazo in https://github.com/hyperledger/bevel/pull/2583
* [indy] refactor codebase for effective deployment by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2587
* [substrate] refactor codebase for effective deployment by @saurabhkumarkardam in https://github.com/hyperledger/bevel/pull/2588
* fabric: hot fix by @mgCepeda in https://github.com/hyperledger/bevel/pull/2590
* shared: update storage class role by @saikumarbommakanti in https://github.com/hyperledger/bevel/pull/2510


**Full Changelog**: https://github.com/hyperledger/bevel/compare/v1.0.0.0...v1.0.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v1.0.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-01 04:29:03 +0000 UTC
    </span>
</div>

