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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    Update service database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace the eservice database with more general service database. That is, replace the old TOML format file with a more persistent LMDB file.
    
The eservice database was limited by what it could store (just enclave services), how it was stored (full file load/save), and how the information was exported.
    
The old eservice database is replaced by a persistent database (implemented with lmdb) that stores information about all services. The database is loaded on first use (similar to the block store manager) from settings in the configuration file.

Note that there are some experimental functions for building plugins that are not expected to persist in their current form.

Note that the eservice database CLI has been replaced with an experimental (and more general) script handler. This is also not expected to persist in its current form.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 15:05:44 +0000 UTC
    </div>
</div>

