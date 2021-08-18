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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    move some hard codings from templates to config_apply.yaml for easy changing behavior
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                related to step1 in #243 ,

admin password and container run command for CA, orderer, peer, couchDB are defined in config_apply.yaml and template files refer them.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 02:48:41 +0000 UTC
    </div>
</div>

