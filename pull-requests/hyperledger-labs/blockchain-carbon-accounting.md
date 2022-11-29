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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/653" class=".btn">#653</a>
            </td>
            <td>
                <b>
                    Update CarbonTracker contract and api-server synchronizer.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update CarbonTracker contract and api-server synchronizer.

Update Carbon Tracker to use ERC 1155 standard instead of ERC 721 to handle both Tracker tokenTypeId=2 as NFT, and ProductToken (tokenTypeId=2) as FT.

New PG DB entities used in Carbon Tracker and ProductToken synchronizer
Introduce new relations for  Carbon Tracker and ProductToken balances
TrackedToken and TrackedProduct relation for NET and ProductToken amounts used to store inputs to Tracker token, respectively.
Introduce CarbonTracker event detection in api-serve synchronizer.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 22:35:52 +0000 UTC
    </div>
</div>

