---
layout: default
title: minifabric
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minifabric
---

# minifabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minifabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    apply the same patch to DockerfileHub for docker image publishing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                followup #225

I noticed that #225 is missing in the latest image in dockerhub.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 23:29:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/225" class=".btn">#225</a>
            </td>
            <td>
                <b>
                    bumps dependent lib versions, to involve latest kubernetes.core and cloud.common
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #224
related to #221

```
new versions:
- ansible:              2.9.x
- openshift:            latest(0.12.1)  from 0.11.2
- community.kubernetes: latest(2.0.0)
- kubernets.core:       latest(2.1.1)
- cloud.common:         latest(2.0.3)
```

with above versions, ansible k8s operation is achieved by redirecting as below:
openshift => community.kubernetes => kubernetes.core => cloud.common
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 07:53:02 +0000 UTC
    </div>
</div>

