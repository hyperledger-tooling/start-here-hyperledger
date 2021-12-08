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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/343" class=".btn">#343</a>
            </td>
            <td>
                <b>
                    Implement wawaka function for parsing an SGX quote & report body
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Add wawaka native function to parse the sgx quote and report
    
Add a function, sgx_parse_report, to convert the binary sgx report into a JSON structure that can be interpreted by the contract. Add a new common function package for processing the sgx attestation. Update the tests for the new values.

Also fix a bug in the error handling of pdo-shell.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 00:09:05 +0000 UTC
    </div>
</div>

