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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    Create key/value store for client use
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Implement python client support for building key value stores
    
In order to share large data structures with a contract, this commit implements support for python to create and send encrypted key value stores.
    
A test script & contract are included to demonstrate how to pass a key value store as a parameter to a contract.

This includes a number of other bug fixes:
* fixes the wawaka system test execution in run-tests.sh
* adds a blockstore "head" operation that returns all metadata
* adds support for replication parameters in pdo-shell
* updates block-store-manager configuration handling
* allow the key prefix in wawaka to be empty
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 23:31:53 +0000 UTC
    </div>
</div>

