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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/359" class=".btn">#359</a>
            </td>
            <td>
                <b>
                    Besu Documentation and RFC Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added `setup-local` and `ledger-initilization` for Besu network asset exchange.
- Restructured `asset-exchange` page, into multiple pages, and added Besu asset exchange instructions.
- RFC updated for Fabric-HTLC
- RFC updated for Corda data sharing
- RFC drafted for Besu data sharing and views.

Deployed new docs: https://sanvendev.github.io/weaver-dlt-interoperability/docs/external/getting-started/guide
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 12:09:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/358" class=".btn">#358</a>
            </td>
            <td>
                <b>
                    Updating Golang package versions and dependencies and Re-enabling workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fabric Interop Chaincode `libs/utils` was upgraded to `1.5.6` earlier. Other packages depending on this library required updates to their dependencies (`go.sum` files).

Re-enabled data sharing and asset transfer workflows dependent on the latest version of the Fabric Interop Chaincode.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 16:06:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/356" class=".btn">#356</a>
            </td>
            <td>
                <b>
                    RFC Improvements and Package Version Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the Fabric Interoperation Chaincode `libs/utils` version.
Fixed permissioning issues in containerized Fabric Driver and Fabric IIN Agent.
Upgraded Fabric testnets to latest Fabric and Fabric-CA versions.
Updated Data Sharing RFCs, partially fixing #238 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 08:55:03 +0000 UTC
    </div>
</div>

