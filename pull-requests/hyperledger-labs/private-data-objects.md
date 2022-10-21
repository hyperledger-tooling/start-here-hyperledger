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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/380" class=".btn">#380</a>
            </td>
            <td>
                <b>
                    Sawtooth in-depth removal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR completes the removal of Sawtooth and depends on #379 for testing (at least the eservice) in HW mode.

This PR removes the following Sawtooth-related things:
- references in docs and toml files
- build flags and procedures
- scripts for SKF files
- configuration flags and procedures in services

Also, it updates:
- the default ledger port 8008 -> 6600
- the default ledger type sawtooth -> ccf
- the registration with the ledger -- which is now empty since CCF is not set up for checking proof-data in HW mode
- the default service keys *.skf -> *.pem
- the TransactionKeys class by deprecating the methods
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 18:56:20 +0000 UTC
    </div>
</div>

