---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Move configuration into scripts that can be installed/run outside the build process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Building the configuration for pdo services, clients and ccf are all buried inside the Makefiles. This makes it challenging to create configuration files for running services. This adds a set of scripts that can be invoked (pdo-configure-services, pdo-configure-client, pdo-configure-ccf) to build the configuration and key files useful for setting up a service or a client.

When configuring services, the tool also creates a "site.toml" file that contains service connection information for all the services. In the future this file can be used to load service information into a client.

**NOTE:** this is not really finished... to be complete a couple additional things must happen:
* CCF must require at least the PDO client to be installed so that pdo-configure-ccf can be called instead of expand-config
* expand-config and make-keys should be removed
* the build/install/configure process must be cleaner in the makefile 

That being said... this should still be useful for building deployable service configurations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 21:31:02 +0000 UTC
    </div>
</div>

