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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/446" class=".btn">#446</a>
            </td>
            <td>
                <b>
                    Legitimately handle versions for packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We have not been very good about version updates. By default the version is extracted from the VERSION file but this requires an explicit commit to update.

This change uses the most recent annotated version tag to determine the major and minor numbers and the commit count to determine that patch number. Future versions should be annotatively tagged as 'vM.N.0'.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 00:20:31 +0000 UTC
    </div>
</div>

