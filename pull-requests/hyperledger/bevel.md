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
                PR <a href="https://github.com/hyperledger/bevel/pull/2226" class=".btn">#2226</a>
            </td>
            <td>
                <b>
                    Added application molecule test in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #738 

Need reviews @sownak @suvajit-sarkar @jagpreetsinghsasan 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 16:17:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2225" class=".btn">#2225</a>
            </td>
            <td>
                <b>
                    [besu] add 'none' as a new option for transaction manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed.**
---
**feat(besu): add 'none' as a new option for transaction manager.**
```
Updated the following files to introduce the new option for transaction manager:
	1. sample network-besu.yaml file.
	2. deployment.yaml file of chart node_besu.
	3. node_besu.tpl template.
```

fixes #2163
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 05:54:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2224" class=".btn">#2224</a>
            </td>
            <td>
                <b>
                    [ci-skip] flux optimisation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    flux optimisation
    - setting up strict flux version while installation
    - skip watching other namespaces
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 05:44:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2223" class=".btn">#2223</a>
            </td>
            <td>
                <b>
                    [ci-skip] Reset network doesn't clean all git release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Fixed deletion of realese files.
2. Fixed issue of detecting the completion of vault-k8s-job 
3 .Fixed undefined variable error in task to check if vault-k8s-job has completed

Modifications in roles and tpl files
-----------------------
platforms/r3-corda/configuration/roles/create/k8_component/Readme.md 
platforms/r3-corda/configuration/roles/create/k8_component/tasks/main.yaml 
platforms/r3-corda/configuration/roles/create/k8_component/vars/main.yaml 
platforms/r3-corda/configuration/roles/create/node_component/Readme.md 
platforms/r3-corda/configuration/roles/create/node_component/tasks/main.yaml 
platforms/r3-corda/configuration/roles/setup/doorman/Readme.md 
platforms/r3-corda/configuration/roles/setup/doorman/tasks/main.yml 
platforms/r3-corda/configuration/roles/setup/nms/Readme.md 
platforms/r3-corda/configuration/roles/setup/nms/tasks/main.yaml 
platforms/r3-corda/configuration/roles/setup/node/Readme.md 
platforms/r3-corda/configuration/roles/setup/node/tasks/main.yaml 
platforms/r3-corda/configuration/roles/setup/notary/Readme.md 
platforms/r3-corda/configuration/roles/setup/notary/tasks/main.yaml 
platforms/r3-corda/releases/README.md
platforms/shared/charts/vault-k8s-mgmt/templates/job.yaml platforms/shared/configuration/roles/check/helm_component/Readme.md platforms/shared/configuration/roles/check/helm_component/tasks/main.yaml platforms/shared/configuration/roles/setup/vault_kubernetes/tasks/main.yaml

Fixes
#2220 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 16:01:10 +0000 UTC
    </div>
</div>

