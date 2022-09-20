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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    Update CarbonTracker contract and documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 Revisions/fixes to contract functions.
  - trackee must be registered industry of NET network
  - simplify productBalance
  - Drop sourceTrackerId mapping. Product's sourceTrackerId is defined in _productData[productId].trackerId 
  - productTransfer() modified
    
Drop function transferProductToTracker(). Superceeded by transferProduct and trackProduct() functions.
 - Owner of audited CarbonTracker contract can transferProduct() to new trackee address.
  - Trackee can trackProduct() received to a new carbon tracker assigned to them.
    
Updated documentation and add diagram to docs/carbon-tracker.md.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 04:37:55 +0000 UTC
    </div>
</div>

