---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/525" class=".btn">#525</a>
            </td>
            <td>
                <b>
                    Refactor reusable code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 12:38:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/524" class=".btn">#524</a>
            </td>
            <td>
                <b>
                    add sql as possible driver for kvs and vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR allows the user to select a golang/sql compatible driver for the vault and key/valuestore as an alternative to Badger. 

Reasons to do that may include:

- Using a managed database for high availability, failover and backups with very little overhead
- Having a stateless instance of the Fabric Smart Client with no filesystem writes and an external database
- The ability to inspect stored data using standard tooling
- Compliance to organization policies

The driver has been tested with the following sql drivers:

- SQLite: (pure go): https://modernc.org/sqlite
- Postgres (pure Go): https://github.com/lib/pq 

Note that for SQLite it's recommended to add a pragma to prevent BUSY_TIMEOUT errors, e.g. `file:/var/fsc/data/fsc.sqlite?_pragma=busy_timeout(5000)`.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 08:26:16 +0000 UTC
    </div>
</div>

