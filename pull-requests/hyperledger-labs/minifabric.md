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
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    fix a bug in abnormal case on k8s environment.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                related to #229,

I met a bug in abnormal case, and fixed it.

In normal case , operator does followings before minifab operation.
A) copy kubeconfig to vars/kubeconfig/config
B) install ingress

abnormal case: operator runs minifab without 'B'

in the above case, current playbook/netdown/k8s-clean-allservices.yaml raises an error.
this PR makes 'minifab cleanup' works without error in the above case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 10:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    remove entries from ingresss k8s in cleanup operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cleaning items,  comparing netup operation:
- entries in tcp-services : YES
- entries in service      : YES
- ingress command args    : NO
    keep '--tcp-services-configmap=...' in ingress controler command args.
    removing command arg causes restarting ingress, it makes down time in other services...

fix #221 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 09:49:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    bump ansible to latest(4.1.0) from 2.9.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                related #224, I succeeded to bump from 2.9.x to latest 4.x.

I felt that minifab processing goes faster...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-27 11:04:49 +0000 UTC
    </div>
</div>

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

