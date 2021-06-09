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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Code Fixes, and new command added to create all credentials for data transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Fixed code getting stuck at end of asset exchange commands.
2. Added sample commands in readme for exchange-step.
3. Added new command `fabric-cli configure create all` to create all credentials (access-control policy, verification policy, membership) and modified interop command to accept user as parameter, in order to remove dependency on using wallet present in repo.
4. Some Typo fixes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 12:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Code Refactoring and Automate deployment of SimpleAsset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Refactored `interface/asset-mgmt` and `simpleasset` to keep unit tests in different package, so that deployment doesn't require mocks to be copied.
2. Automated copying of `asset-mgmt` into `simpleasset` during network deployment.
3. Added a clean target in `interoperation-node-sdk`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 18:35:29 +0000 UTC
    </div>
</div>

