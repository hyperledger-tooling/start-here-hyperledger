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
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    Update tests for the service groups database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace invocation of the script for building a local groups and services database with one that uses the public interfaces for the services and groups databases. Move away from "host specific" configuration to a configuration based on the more general site configuration file (i.e. site.toml).
    
By default, testing will still occur with locally hosted services. Importing a site configuration file from another service provider (which just involves copying the site configuration file to ${PDO_HOME}/etc/sites/${SERVICE_HOST}.toml) enables use of PDO services from any location.

This is a draft until the corresponding PR (https://github.com/hyperledger-labs/private-data-objects/pull/481) is committed to PDO. Before it is committed, the private-data-object submodule must be updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 15:34:22 +0000 UTC
    </div>
</div>

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

