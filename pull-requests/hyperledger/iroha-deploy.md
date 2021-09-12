---
layout: default
title: iroha-deploy
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-deploy
---

# iroha-deploy <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-deploy){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-deploy/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    [DOPS-1451] Fix Iroha deploy role
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Task
[DOPS-1451]: Fix iroha-deploy role
depending on version (ansible or docker) Iroha role fails with error:
`iroha_command_register.ansible_facts.docker_container.Output` - is not defined
this is the old name for variable, the new one look like that: `iroha_command_register.container.Output`

## Changes
1. tasks to support new format of the variable  has been fixed
2.  the task to check  that we can run role on new version of Ansible has been added

## Author
Signed-off-by: Vasiliy Zyabkin zyabkin@soramitsu.co.jp
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-11 21:31:58 +0000 UTC
    </div>
</div>

