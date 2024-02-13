---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2507" class=".btn">#2507</a>
            </td>
            <td>
                <b>
                    update(docs): Indy configuration and ops sections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Primary Changes**

1. Updated operations Indy docs
2. Updated Indy config file
3. Added missing field (proxy_namespace) in Substrate

fixes #2465 #2483
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 12:44:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2506" class=".btn">#2506</a>
            </td>
            <td>
                <b>
                    docs(r3corda): operations section under guide's tab
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Primary Changes**
1.Updated operations corda docs
2.Removed cenm console in corda operations

fixes #2483
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 06:33:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2505" class=".btn">#2505</a>
            </td>
            <td>
                <b>
                    [corda] New charts as per release 1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New 1.0.0 changes
- Added kubectl to bevel-build container
- Updated `platforms/r3-corda/charts/README.md` to guide on how to deploy using just helm install
- All `platforms/r3-corda/charts/` updated to use global variables
- New chart `platforms/r3-corda/charts/corda-init` to initialise a namespace for Corda
- New Chart `platforms/r3-corda/charts/corda-network-service` to deploy Doorman, NMS and MongoDB together
- Removed doorman, mongodb, and nms charts
- Updated `platforms/r3-corda/charts/corda-node` chart to deploy notary as well. Also deploys H2 database.
- Removed Notary and init-registration charts
- Hooks used to create certificates
- All passwords are in values.yaml files now
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 11:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2504" class=".btn">#2504</a>
            </td>
            <td>
                <b>
                    docs(quorum): configuration section under guides tab
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                changes:

Configurations:
networkyaml-quorum.md

fixes:2465
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 13:40:53 +0000 UTC
    </div>
</div>

