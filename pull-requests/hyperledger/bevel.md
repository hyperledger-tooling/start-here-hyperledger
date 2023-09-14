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

