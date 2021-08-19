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
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    update docs/DeployOntoK8S.md for reordering instrucction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                proxy environment variable is set     x after ingress install    o before ingress install

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 08:11:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    reuse task with vars to clean k8s ingress entries.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                before:
```yaml
  include_tasks : playbooks/ops/xxx/k8s-clean-service.yaml
  # port list  is embeded in the above file
```
after:
```yaml
 inlcude_tasks: playbooks/common/k8s-rm-ingress-entry.yaml
 vars: 
   ours: "{{ [ list of ports we want to remove from ingress controller ] }}"
```
playbooks/common/k8s-rm-ingress-entry.yaml is involved previous PR 253
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 04:49:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    portainer support for kubernetes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                portainer's k8s supporting, based on https://github.com/portainer/k8s/blob/master/deploy/manifests/portainer/

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 06:22:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    Explorer support for Kubernetes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #245
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 00:00:21 +0000 UTC
    </div>
</div>

