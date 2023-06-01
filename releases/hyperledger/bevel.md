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
                    Bevel Release 0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.14.0.0
                </span>
            </td>
            <td>
                ## What's new in Bevel
- Added support for substrate based DSCP platform
- Added support for deployment on Kubernetes v1.23
- New repository created bevel-samples to host reference application

## New Features
- HL Fabric
  - Moved create/user role to Kubernetes jobs
  - Enabled Cacti Connector deployment
- HL Besu
  - Moved create/crypto role to Kubernetes jobs
  - Enabled Cacti Connector deployment
  - Enabled node permissioning and monitoring
  - Transaction manager 'none' option for disabled privacy
  - Support for labels in deployment and service
- Quorum 
  - Transaction manager 'none' option for disabled privacy 
## Deprecation
  - No active support for older versions of platforms. Check [compatibility matrix](https://blockchain-automation-framework.readthedocs.io/en/latest/compatibilitymatrix.html)
## Major Bug Fixes
  -  Fixed fabric running upgrading from 1.4.x to 2.2.x using incorrect flag condition #2142
  -  Fixed intermittent flux installation/uninstallation issues #2157
  -  Fixed join channel job not starting #2212
  -  Fixed add org for proxy none for fabric platform #2274

## Known issue
- Flux uninstallation taking longer time

## Improvements
- Besu
    - Refactor genesis creation and crypto creation
    - Single vault management script for sidecar containers
- Quorum
    - Refactor "tessera" role to move node creation logic to separate role.
- Shared
    - Created bevel-alpine-ext image with mysql
## Documentation
- Added cacti connector operations for HL Besu and HL Fabric platform
## Application
- Added deployment of supplychain smart contract automation for Besu

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/v0.14.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    tessera_key_mgmt-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    tessera_key_mgmt-0.14.0
                </span>
            </td>
            <td>
                A Helm3 chart for generating Tessera crypto
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/tessera_key_mgmt-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    orion_key_mgmt-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    orion_key_mgmt-0.14.0
                </span>
            </td>
            <td>
                A Helm3 chart for generating Orion crypto
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/orion_key_mgmt-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    node_validator-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    node_validator-0.14.0
                </span>
            </td>
            <td>
                A Helm chart to deploy Hyperledger Besu nodes with orion transaction manager
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/node_validator-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    node_tessera-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    node_tessera-0.14.0
                </span>
            </td>
            <td>
                A Helm chart to deploy Tessera transaction manager nodes
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/node_tessera-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    node_orion-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    node_orion-0.14.0
                </span>
            </td>
            <td>
                A Helm chart to deploy Hyperledger Besu nodes with orion transaction manager
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/node_orion-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    node_key_mgmt-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    node_key_mgmt-0.14.0
                </span>
            </td>
            <td>
                A Helm chart to perform node key generation
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/node_key_mgmt-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    node_besu-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    node_besu-0.14.0
                </span>
            </td>
            <td>
                A Helm chart to deploy Hyperledger Besu nodes
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/node_besu-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    generate_ambassador_certs-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    generate_ambassador_certs-0.14.0
                </span>
            </td>
            <td>
                A Helm3 chart for generating ambassador certificates
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/generate_ambassador_certs-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    besu_connector-0.14.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    besu_connector-0.14.0
                </span>
            </td>
            <td>
                A Helm chart for Cactus Besu Connector
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/bevel/releases/tag/besu_connector-0.14.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-01 19:15:32 +0000 UTC
    </span>
</div>

