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
                     Bevel Release 0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.15.0.0
                </span>
            </td>
            <td>
                ## What's new in Bevel
- Cacti quorum connector
- Proxy ambassador upgraded to latest ambassador edge stack
- Support for chaincode as an external service
- Helm charts published on github hosted helm repo using github pages
- Option on Bevel to deploy the Fabric network using bevel-operator-fabric
- Support Fabric v2.5 network deployment

## New Features
- HL Fabric
  -  One organization-multiple cluster deployments support
- HL Besu
  - Prometheus integration for Besu node monitoring

## Deprecation
  - No active support for older versions of platforms (below v0.13)
  - Molecule testing support is removed 
## Major Bug Fixes
  - Besu addition of the new org fails #2316 

## Improvements
  - Single vault management script for sidecar containers
  - Update security context in helm charts
  - Creation of vault auth from shared vault-k8s chart
  - Creation of storgeclass from shared storageclass chart
  - Fabric: Remove hardcoding of 8443 port and introduce an OrdererAddress
  - Ansible roles readme removed, inline code comments added
  - Platform chart names refactored to fix name conficts
## Documentation
- Minikube doc and general documentation improvements 
- Besu onchain permission guide

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v0.15.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu_connector-0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu_connector-0.15.0
                </span>
            </td>
            <td>
                Hyperledger Besu: Deploys Cactus Besu Connector
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu_connector-0.15.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu-validator-node-0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu-validator-node-0.15.0
                </span>
            </td>
            <td>
                Hyperledger Besu: Deploys Hyperledger Besu validator nodes
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu-validator-node-0.15.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu-tlscert-cert-gen-0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu-tlscert-cert-gen-0.15.0
                </span>
            </td>
            <td>
                Hyperledger Besu: Generates and stores ambassador certificates
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu-tlscert-cert-gen-0.15.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu-tessera-node-0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu-tessera-node-0.15.0
                </span>
            </td>
            <td>
                Hyperledger Besu: Deploys Tessera transaction manager nodes
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu-tessera-node-0.15.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu-tessera-key-mgmt-0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu-tessera-key-mgmt-0.15.0
                </span>
            </td>
            <td>
                Hyperledger Besu: Generates and stores Tessera cryptographic materials
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu-tessera-key-mgmt-0.15.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu-node-key-mgmt-0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu-node-key-mgmt-0.15.0
                </span>
            </td>
            <td>
                Hyperledger Besu: Generates and stores node cryptographic materials
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu-node-key-mgmt-0.15.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu-member-node-0.15.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu-member-node-0.15.0
                </span>
            </td>
            <td>
                Hyperledger Besu: Deploys Hyperledger Besu nodes
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu-member-node-0.15.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-08 20:39:21 +0000 UTC
    </span>
</div>

