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
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/42" class=".btn">#42</a>
            </td>
            <td>
                <b>
                    Add component actions and updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds the following to allow component actions (restart, reenroll, etc)
- certificate_authority_action
- ordering_service_node_action
- peer_action

This change also updates the update methods for peer, CA and ordering service nodes to allow for V3 APIs.

There is also an added capability to list associated notes with a CA:
- certificate_authority_associated_nodes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-20 16:53:37 +0000 UTC
    </div>
</div>

