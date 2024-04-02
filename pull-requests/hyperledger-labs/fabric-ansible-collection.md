---
layout: default
title: fabric-ansible-collection
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-ansible-collection
---

# fabric-ansible-collection <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-ansible-collection){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    strip the 'v' prefix that newer fabric binaries print as their versio…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …n, to prevent LooseVersion comparison breakage
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 10:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Update actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-29 14:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Solve error related to running the ansible collections when using the default docker entrypoint linked to ibp-user
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to issue: #43

Added new docker entrypoint to be able to override the current one.

The error happens when we follow the documentation from the public repository for running the playbooks with the docker image:

```bash
docker pull ghcr.io/hyperledger-labs/fabric-ansible:sha-c9330b9
docker run --rm -u $(id -u) -v /path/to/playbooks:/playbooks ghcr.io/hyperledger-labs/fabric-ansible:sha-c9330b9 ansible-playbook /playbooks/playbook.yml
```
Error:

```bash
Traceback (most recent call last):
  File "/home/hlf-user/.local/bin/ansible-playbook", line 5, in <module>
    from ansible.cli.playbook import main
ModuleNotFoundError: No module named 'ansible' 
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-29 03:01:14 +0000 UTC
    </div>
</div>

