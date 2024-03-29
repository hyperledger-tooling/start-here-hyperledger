---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Complete several of the utility documents for Jupyter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds support for several utility notebooks that can be used for managing a client configuration. The notebooks themselves are included along with a collection of widgets that can be used by contract-specific notebooks. The widgets generally include ones to create lists of available resources (e.g. keys, services, groups), select amongst a list of available resources, and create or update resources.

* key-manager: manage keys available to the client
* service-manager: manage the database of services that can be used for contracts
* service-groups-manager: manage the database of service groups used for contracts

Note that this PR assumes that PDO PR https://github.com/hyperledger-labs/private-data-objects/pull/481 has been applied. Until that PR is merged and the private-data-objects submodule has been updated, this will remain a draft.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-29 16:32:20 +0000 UTC
    </div>
</div>

