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
                PR <a href="https://github.com/hyperledger/bevel/pull/2313" class=".btn">#2313</a>
            </td>
            <td>
                <b>
                    [ci-skip] Add operator support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">fabric</span>
            </td>
            <td>
                This PR adds support for bevel-operator-fabric in traditional Bevel using Ansible. gitops and vault is optional, but proxy = none is not supported because bevel-operator-fabric itself has istio as mandatory.
This PR adds support till channel creation and joining, chaincode management is not supported.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 14:55:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2312" class=".btn">#2312</a>
            </td>
            <td>
                <b>
                    [ci-skip] make docker credentials section optional in network.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request aims to make the Docker credentials section optional in the network.yaml file of Hyperledger Fabric. By doing so, will have the flexibility to include or exclude the Docker credentials based on the deployment requirements.

Changes Made:
1. Made the docker username and passsword section optional by allowing us to exclude it or leave it empty if not required.
2. Updated the relevant charts and tpl files to reflect the optional docker credentials section.
3. In the file Hyperledger-fabric/configuration/roles/setup/vault Kubernetes/tasks/main.yaml, docker pull credentials are only created when a specific condition is met.

Fixes: #613
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 13:10:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2311" class=".btn">#2311</a>
            </td>
            <td>
                <b>
                    [ci-skip] utilize the common vault-k8s-mgmt Helm chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(shared): utilize shared vault-k8s-mgmt Helm chart for Fabric and R3-Corda-Ent platforms.**
```
This commit implements the following changes:

- Updated the shared role setup/vault-kubernetes to support both the Fabric and R3-Corda-Ent platforms.
- Implemented vault policy templates, fabric-policy.tpl and r3-corda-ent-policy.tpl, for Fabric and R3-Corda-Ent respectively.
- Updated the variables in the shared role setup/vault_kubernetes to ensure compatibility with both the Fabric and R3-Corda-Ent platforms.
- Removed the setup/vault-kubernetes from the Corda platform, enabling the use of the shared role setup/vault-kubernetes for the same purpose.
- Removed the setup/vault-kubernetes from the Fabric platform, enabling the use of the shared role setup/vault-kubernetes for the same purpose.
- Removed the Helm Chart vault_kubernetes from the Fabric platform, enabling the use of the shared Helm Chart vault-k8s-mgmt.

These changes enable code reuse and ensure consistency across the Fabric and R3-Corda-Ent platforms, as both now utilize the shared vault-k8s-mgmt Helm chart.
```

fixes #2291
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 11:07:25 +0000 UTC
    </div>
</div>

