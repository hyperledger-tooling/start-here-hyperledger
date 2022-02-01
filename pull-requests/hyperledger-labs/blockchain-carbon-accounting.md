---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    feat(chaincode): Use OrbitDB to load emissions factors instead of CouchDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a work in progress to use the emissions factors loaded in OrbitDB (#321) instead of using Mango queries to access the emissions factors stored on CouchDB. This PR refactors the chaincode to call OrbitDB instead of CouchDB, without modifying the chaincode's API. However, due to a dependency conflict, (viz. OrbitDB requires Node >= v16 whereas the Fabric peer running the chaincode runs on Node v12.16.1, without having a clear way to configure the peer to use the required version of Node) running the chaincode fails.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 17:46:00 +0000 UTC
    </div>
</div>

