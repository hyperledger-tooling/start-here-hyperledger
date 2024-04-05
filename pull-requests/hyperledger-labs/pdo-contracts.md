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
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Enable starting guardian sservice at specified interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes it possible to start guardian sservice at the specified interface rather than default localhost

Signed-off-by: Prakash Narayana Moorthy <prakash.narayana.moorthy@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 19:30:41 +0000 UTC
    </div>
</div>

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

