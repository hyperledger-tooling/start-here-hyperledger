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
                PR <a href="https://github.com/hyperledger/bevel/pull/2369" class=".btn">#2369</a>
            </td>
            <td>
                <b>
                    [quorum] Upgrade and Add support for Ambassador v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add support for Ambassador v3 in Quorum
- Remove constellation support
- Update Quorum to latest 23.4.0 version
- Remove support for older versions of Quorum and Besu
- Update Vault-k8s-job to create Vault auth correctly
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 09:55:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2368" class=".btn">#2368</a>
            </td>
            <td>
                <b>
                    [besu] enable one prometheus for all organizations of a network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(besu): enable one prometheus for all organizations of a network**

```
This pull request enables one Prometheus server to be used for all organizations in a network.

Changes:
 • The Prometheus code has been migrated to the setup-k8s-environment.yaml playbook in the shared platform.
 • Unwanted variables have been removed from the Prometheus Ansible role.
 • The Prometheus code has been modified to first fetch all the targets from different organizations and then deploy Prometheus in the default namespace with the same fetched targets.
 • Introduced "prometheus-routing.tpl" file to create Ambassador routing rules dynamically for the Prometheus server.

Benefits:
 • This feature reduces the complexity of managing Prometheus by eliminating the need to deploy separate Prometheus servers for each organization.
 • It also improves the efficiency of Prometheus by allowing it to collect metrics from all organizations in a single place.
```

fixes #1416
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 12:18:37 +0000 UTC
    </div>
</div>

