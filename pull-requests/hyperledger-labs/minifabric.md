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
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    fix java chaincode to work with current fabric versions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #260
tested and worked with following fabric versions
- 1.4.4 (current minimum supported version by minifab)
- 2.0    ( first 2.0 series)
- 2.3.2 ( latest )

so, other version can work with this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-22 04:13:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    Change latest Fabric version from 2.2.0 to 2.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed the current Fabric release version number in the docs from 2.2.0 to 2.3.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 23:08:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    Fixed issue described in issue 257
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tong Li <litong01@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 12:28:01 +0000 UTC
    </div>
</div>

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

