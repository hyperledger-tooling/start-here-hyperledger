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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    Tutorial updates, and RFC, bug and package version fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Edited the Weaver Enablement for Fabric tutorial page, adding more context and providing explicit instructions to enable TLS among connections across relays, drivers, and IIN Agents (partly fixing #257 )
- Fixed bad links in various RFCs.
- Fixed data sharing workflow bug.
- Updated some Go module package dependencies to latest versions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 20:50:10 +0000 UTC
    </div>
</div>

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

Update:
- Updated Corda asset exchange in "Enable weaver in your application" document.

Update 2:
- Support an array of payloads, one from each node in Corda View.
- Updated rfc, core contracts, and SDK as per above Corda View change.
- Added 2 orgs test in Corda Interop App unit test, and fixed bug in ViewVerification when receiving view from 2 orgs.
- All modules updated to `v1.5.7` except corda modules which are updated to `v1.2.13`

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

