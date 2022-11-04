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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/646" class=".btn">#646</a>
            </td>
            <td>
                <b>
                    Updates to methane app & fix for typescript-app-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See [app/methane/README.md](https://github.com/net-zero-project/blockchain-carbon-accounting/blob/main/app/methane/README.md) for updates to Methane (Oil & Gas Emissions) app

+Fix to fails in test-typescript-app CI. Changes in how GitHub was handling actions prevented docker containers from reaching localhost using docker-compose.yml option.
```
 extra_hosts:
            - "host.docker.internal:host-gateway"
```
Fixed by moving all processes to docker,  i.e.,  api-server used by fabric chain-code [oracle service](https://github.com/net-zero-project/blockchain-carbon-accounting/tree/main/app/api-oracle#readme) to calculate emissions from postgres DB. New environment variable START_SERVER=true used to run the api-server with SKIP_SYNC=true (no need to sync with the local hardhat network)

The oracle also runs as a container attached to Fabric network
both api-server and oracle-api container images are hosted under the [net-zero-project ghcr.io](https://github.com/orgs/net-zero-project/packages) until hosting permission are granted under hyperledger-labs

#Oil & gas portal

emissions and production data points from multiple sources for oil & gas operators. Allow users to view individual asset and aggregate data points for a given operator.

Users can request emission audits for an existing (unverified) carbon tracker token using single or multiple data points to identify discrepancies in different sources.

Single data points are handled as the new industry activity_types using process_industry method of supply-chain-lib

Multiple-data points are submitted using the other activity_type from react-app RequestAudit form. A local file is generated with each row of product data selected for the request, plus the requested carbon tracker ID.

Auditors can also assign production data (oil and gas quantities) as described in the Carbon Tracker contract [Readme](https://github.com/hyperledger-labs/blockchain-carbon-accounting/blob/main/hardhat/docs/carbon-tracker.md)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 06:56:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/644" class=".btn">#644</a>
            </td>
            <td>
                <b>
                    remove more private key in client features
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
        Created At 2022-11-02 16:29:43 +0000 UTC
    </div>
</div>

