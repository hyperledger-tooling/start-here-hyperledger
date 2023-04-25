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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    Enable service groups to be configured through toml files rather than built exclusively in the site.psh script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Service configuration groups are a convenient way to group parameters when creating contracts. Currently we require the groups to be reconfigured through site.psh on every script invocation. Maintaining the groups is very tightly connected with maintaining site.psh (which also loads a limited set of services into the eservice database).

This PR adds a pdo-shell command for importing and exporting service groups through a toml file. The intent is that groups can be added through a configuration file rather than editing the script every time. The script interface still works (none of the commands have been removed); whats new is the batching.

Several other small fixes added along the way as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 17:15:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/434" class=".btn">#434</a>
            </td>
            <td>
                <b>
                    Allow replication service to limit the duration of cached blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The current policy for storage services is that the client determines the length of time a block will be stored. This is rather unrealistic. This makes the maximum duration a configuration parameter in the storage service and enforces the limit. The default value of 0 for the duration perserves the current behavior (the client determines the length of time the storage service will hold the block).

Note that this will require some adaptation when the replication policy is enforced by the ledger.

Also note that the automated tests are insufficient for testing at this point. The simplest test is to edit the test configuration files for sservice[2-5].toml and set the garbage collect interval to 1 and the max duration to 1, then run the services test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 16:33:14 +0000 UTC
    </div>
</div>

