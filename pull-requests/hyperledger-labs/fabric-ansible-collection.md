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
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Fixed naming of the collection following change in the galaxy.yml file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The galaxy.yml file was changed at some point to rename the collection to `fabric_ansible_collection`:

https://github.com/hyperledger-labs/fabric-ansible-collection/blob/371e5665bc8c6f99ea4f648bedda7b8893c85aee/galaxy.yml#L6

However some of the roles and the tutorial playbooks referred to it with dashes instead of underscores, eg:

https://github.com/hyperledger-labs/fabric-ansible-collection/blob/371e5665bc8c6f99ea4f648bedda7b8893c85aee/roles/endorsing_organization/tasks/create.yml#L41

This meant locally built Ansible collections would not work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 09:00:48 +0000 UTC
    </div>
</div>

