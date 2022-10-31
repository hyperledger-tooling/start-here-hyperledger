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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/642" class=".btn">#642</a>
            </td>
            <td>
                <b>
                    Methane app updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates to methane app client and server

See [app/methane/README.md](https://github.com/net-zero-project/blockchain-carbon-accounting/blob/main/app/methane/README.md)

Oil and gas database includes emission and production data points from different sources.

Users can request emission audits submitted to a carbon tracker using single or multiple data points used to evaluate an operators total emissions.

Single data points are handled as the new industry activity_types using process_industry method of supply-chain-lib

Multiple-data points are submitted using the other activity_type using the react-app RequestAudit form. A local file is generated as a stringified list of all the JSON Product data points, and the requested tracker ID.

Auditors can also assign production data (oil and gas quantities) as described in the Carbon Tracker contract [Readme](https://github.com/hyperledger-labs/blockchain-carbon-accounting/blob/main/hardhat/docs/carbon-tracker.md)

This PR also implements the oracle api service as a docker container when running the Fabric network.
The image is temporarily hosted under the [net-zero-project ghcr.io](ghcr.io/net-zero-project/blockchain-carbon-accounting/oracle-api:latest) until hosting permission are granted under hyperledger-labs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-28 04:17:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    remove some code for private key #638
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
        Created At 2022-10-26 16:03:30 +0000 UTC
    </div>
</div>

