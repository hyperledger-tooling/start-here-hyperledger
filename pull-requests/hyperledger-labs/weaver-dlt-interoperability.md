---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Restructure Asset Exchange Library and Fix ContractID APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Restructure AssetExchange lib, split the code into multiple files:
    - assetSwapContracts.go: HTLC functions: lock, claim, unlock and isLocked functions go here 
    - types.go: all constants, data structures and interface go here.
    - utility.go: all good to have utility HTLC functions go here.
    - helpers.go: all common helper functions go here.
    - idGenerator.go: functions to generate keys for different purposes go here.
- Moved common claim and unlock operations in a separate function, to reduce redundancy.
- Made contractId APIs work for fungible assets as well.
- Added Badge for Besu Asset exchange, re-ordered the badges, and added link to each badge to workflow action.

Closes #366 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 18:15:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/365" class=".btn">#365</a>
            </td>
            <td>
                <b>
                    Fix node pkgs deploy workflow and update jsrsasign package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #363 
Signed-off-by: sandeep.nishad1 <sandeep.nishad1@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 08:38:05 +0000 UTC
    </div>
</div>

