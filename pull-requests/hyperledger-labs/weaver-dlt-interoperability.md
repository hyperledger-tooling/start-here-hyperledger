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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Feature to select Endorsing Orgs in Fabric Data Sharing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added list of orgs as parameter in `interopFlow` in SDK to chose endorsing orgs.
2. Added `participants` field under `ContractTransaction` in events.proto.
3. Updated fabric-driver `writeExternalState` endpoint to allow use of list of orgs to submit transaction to in case of event publication.
4. Updated the way to update docker images version using `VERSION` file (making it uniform with go modules).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 06:04:28 +0000 UTC
    </div>
</div>

