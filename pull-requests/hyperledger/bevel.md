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
                PR <a href="https://github.com/hyperledger/bevel/pull/2466" class=".btn">#2466</a>
            </td>
            <td>
                <b>
                    fix(fabric): correct path for core.yaml file; remove cc ops from site.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 06:33:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2464" class=".btn">#2464</a>
            </td>
            <td>
                <b>
                    feat(besu): enable DLT deployment via GitHub Workflow & Action.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes:

Introduced a new GitHub Workflow enabling the deployment of Hyperledger Bevel's BESU DLT Platform to an EKS Cluster. Introduced a new directory at path: platforms/hyperledger-besu/configuration/samples/workflow, containing two new sample network configuration files: 
network-proxy-besu: Supports deployment with Ingress controller. 
network-no-proxy-besu: Supports deployment without an Ingress controller, specifically designed for deployment on Minikube.

Additional Changes:

1)Replaced the Ambassador Ansible task with new Ambassador-Edge-Stack. 
2)platforms/shared/charts/bevel-vault-mgmt/templates/serviceAccount.yaml 3)platforms/shared/configuration/roles/setup/kubectl/tasks/main.yaml

fixes #2416
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-02 09:55:05 +0000 UTC
    </div>
</div>

