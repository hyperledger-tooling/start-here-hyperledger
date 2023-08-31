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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/447" class=".btn">#447</a>
            </td>
            <td>
                <b>
                    Replace the eservice json database with a more functional database that can be used for all service types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace the eservice database with more general service database

The eservice database was limited by what it could store (just enclave services), how it was stored (full file load/save), and how the information was exported.
    
The old eservice database is replaced by a persistent database (implemented with lmdb) that stores information about all services. The database is loaded on first use (similar to the block store manager) from settings in the configuration file.

The eservice_db pdo-shell command is replaced with one for all service databases (using the new format).
    

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 15:06:12 +0000 UTC
    </div>
</div>

