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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    Fabric Interoperation Chaincode Upgrade for Attested Foreign Identities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                After introducing IIN agents as the decentralized identity and credential managers for security domains' members, foreign memberships cannot be recorded on local ledgers without adequate attestations and authentication checks. This PR adds the following:
- Updates to the membership portion of the Fabric Interoperation Chaincode to handle counter attested memberships of the kinds that will be generated after local and IIN agents go through a sync-and-sign protocol.
- Updates to common identity protos
- Fabric CLI upgrade to handle counter attested memberships
- RFC updates: primarily terminology and language fixes.

Fixes #309 and #315 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 07:25:38 +0000 UTC
    </div>
</div>

