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
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    feature: persist fabric-ca data on k8s.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                as the same as docker, let us persist fabric-ca data on k8s.

```
# on docker ( playbooks/ops/netup/dockerapply.yaml )
- name: Start all ca nodes
  command: >-
    docker run -d --network {{ NETNAME }} --name {{ item.fullname }} --hostname {{ item.fullname }}
    :
    -v {{ item.fullname }}:/etc/hyperledger/fabric-ca-server ## <- persisting CA data
    {{ container_options }}
    hyperledger/fabric-ca:{{ desiredrelease }}
 
# on k8s (playbooks/ops/netup/k8stemplates/allnodes.j2)
containers:
 - name: {{ nodename }}
   image: hyperledger/fabric-ca:1.4
      :
   volumeMounts:
    - { mountPath: "/etc/hyperledger/fabric-ca/idcerts", name: "cert-key-id" }
   # !!! no volume mount for CA data (/etc/hyperledger/fabric-ca-server), let's persist it.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 14:01:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    fix reflecting environment variables in fabric-ca container from spec.yaml on k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes following issue on k8s.
on k8s, environment variables in spec.yaml are reflected in orderer and peer but not in CA.
on the other hand, on docker, all environment variables in spec.yaml are reflected in corresponding container.

with this PR, all environment variables are reflected from spec.yaml in corresponding container on k8s, as the same as docker.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 03:35:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    fix fabric-orderer TLS certs for k8s.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #207
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 15:29:11 +0000 UTC
    </div>
</div>

