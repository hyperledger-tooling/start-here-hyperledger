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
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    improving on-premise k8s uses.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * supporting local-path-provisioner, for persistent storage.
  local-path-provisioner seems not support 'subPath' for volumeMounts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 05:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    new feature for k8s, deploying pod(container) to the specific node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                current minifabric cannot control pod and node binding.
as the result, the peer and it's backend couchdb may be deployed on different worker node,
same situation occurs between peer's CA and peer.
That is not good from point of view of performance or isolation.

This feature involves nodeAffinity with preferredDuringSchedulingIgnoredDuringExecution.
refer https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/

in short,
 - It makes k8s deploy each pod to the specific node according to node labels.
 - k8s deploys a pod in default manner, in following cases:
      - if corresponding label is not assigned in any nodes.
      - if destination node reached to the max-pods-per-node limitation

three types of label are involved:
 * type A (strongest; dock.hlf-fqdn/*) : fully control one pod by one pod
 * type B (2nd; dock.hlf-type/*) : type by type (peer, orderer, ca, couchdb)
 * type C (3rd; dock.hlf-dn/*)    : domain by domain (org0.example.com, org1.example.com)

This feature provides you a way to control pod and node binding, by your assigning labels to nodes.
if you omit assigning labels, k8s deploys pods according to the default manner, as before.

check docs/DeployOntoK8S.md for detail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 10:55:17 +0000 UTC
    </div>
</div>

