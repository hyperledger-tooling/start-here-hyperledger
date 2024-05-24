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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Improved cmake for generating the configuration file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update cmake macros for more consistent processing of SGX configuration
    
    * Simplify and document the PDO_DEBUG_BUILD configuration checks
    * Move all of the configuration template processing into a single cmake FUNCTION
    * Cmake now uses the configure_file command to perform variable substitution (no more sed)
    

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-22 23:54:53 +0000 UTC
    </div>
</div>

