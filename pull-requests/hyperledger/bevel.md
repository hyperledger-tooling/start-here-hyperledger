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
                PR <a href="https://github.com/hyperledger/bevel/pull/2463" class=".btn">#2463</a>
            </td>
            <td>
                <b>
                    [fabric] Hotfix init required
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Primary Changes**

1. Added the init_required field in the tpl files.
2. Fixed error in the invoke chaincode job.
3. Fixed errors in variable names.

**Modifications**
platforms/hyperledger-fabric/charts/fabric-chaincode-commit/templates/commit_chaincode.yaml
platforms/hyperledger-fabric/configuration/roles/create/chaincode/invoke/tasks/nested_valuefile.yaml
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/approve_chaincode_job.tpl
platforms/hyperledger-fabric/configuration/roles/helm_component/templates/commit_chaincode_job.tpl
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-27 16:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2462" class=".btn">#2462</a>
            </td>
            <td>
                <b>
                    [quorum] enable DLT deployment via GitHub Workflow & Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(quorum): enable DLT deployment via GitHub Workflow & Action

Changes:

Introduced a new GitHub Workflow enabling the deployment of Hyperledger Bevel's QUORUM DLT Platform to an EKS Cluster.
Introduced a new directory at path: platforms/quorum/configuration/samples/workflow, containing two new sample network configuration files:
network-proxy-quorum: Supports deployment with Ingress controller.
network-no-proxy-quorum: Supports deployment without an Ingress controller, specifically designed for deployment on Minikube.
Additional Changes:

Replaced the Ambassador Ansible task with new Ambassador-Edge-Stack.

fixes https://github.com/hyperledger/bevel/issues/2416
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-26 19:08:55 +0000 UTC
    </div>
</div>

