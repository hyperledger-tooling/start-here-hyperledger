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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/373" class=".btn">#373</a>
            </td>
            <td>
                <b>
                    feat (test): Test if emission factors for the correct region are used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR modifies the test setup script to insert emission factors for Germany, along with a utility identifier in the same region. Then, 2 emissions are recorded, one in the region of Germany, and the other in the US. Then we assert the following conditions:

- The emissions amounts of both years must not be equal
- The emissions amounts of each region should match the value calculated as per the emissions factors of that year
- In case of the emission recorded in Germany, the amounts of renewable and non-renewable energy must also match the values calculated as per the percent of renewables used in the region
- The emissions data is fetched from the CouchDB database using the HTTP /db/_find API. Then, the emissions factors are calculated and checked against the values stored on the ledger.

Closes #317.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 19:00:18 +0000 UTC
    </div>
</div>

