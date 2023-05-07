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
                PR <a href="https://github.com/hyperledger/bevel/pull/2232" class=".btn">#2232</a>
            </td>
            <td>
                <b>
                    Add check-in condition "[indy]" for Indy test in PR title 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #734
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-07 07:30:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2231" class=".btn">#2231</a>
            </td>
            <td>
                <b>
                    [besu] Add extradata field in genesis file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Add extradata field in genesis file. platforms/hyperledger-besu/configuration/roles/create/genesis role
2. Fixed duplicate app label in platforms/hyperledger-besu/charts/generate_ambassador_certs

Modifications in roles and tpl files
-----------------------
platforms/hyperledger-besu/charts/generate_ambassador_certs/templates/job.yaml 
platforms/hyperledger-besu/configuration/roles/create/genesis/ibft/tasks/main.yaml
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 08:25:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2230" class=".btn">#2230</a>
            </td>
            <td>
                <b>
                    [shared ]: fix job retries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change Log

- fix job retries
#2229 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 12:52:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2228" class=".btn">#2228</a>
            </td>
            <td>
                <b>
                    [ci-skip] add app labels on helm chart jobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change log**

- Fixes retry exhaust on job check roles
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 07:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2227" class=".btn">#2227</a>
            </td>
            <td>
                <b>
                    [ci-skip] Revert "flux optimisation"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/bevel#2224

Helm releases are not getting installed post this change, reverting the PR. Kindly test and and create PR. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 07:44:25 +0000 UTC
    </div>
</div>

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
	
In addition to the above changes, I also made the following updates:
	1. added a label to the job.yaml file of the generate_ambassador_certs chart
	2. corrected playbook names in the add-new-organization.yaml file
```

fixes #2163
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 05:54:28 +0000 UTC
    </div>
</div>

