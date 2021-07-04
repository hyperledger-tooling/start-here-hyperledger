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

