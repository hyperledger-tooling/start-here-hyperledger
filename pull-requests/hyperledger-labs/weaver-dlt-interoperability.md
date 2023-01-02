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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/354" class=".btn">#354</a>
            </td>
            <td>
                <b>
                    Data Sharing Protocol Bug Fixes and RFC Specification Improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixed the Fabric view structure and the associated proof collection and validation logic to take into account the fact that different proof-generating peers may produce and sign different blobs representing the same underlying data (because protobuf serialization and data encryption are typically non-deterministic). This required changes to the common protobufs, the Fabric Driver, the Fabric Interoperation Chaincode, and the Fabric Interoperation Node SDK. (The Fabric Interoperation Go SDK will be updated at a later date along with various other feature upgrades.) This fixes #350 and #351 .

Images were fixed to be rendered properly on dark backgrounds as required by #260 .

Asset transfer RFC specifications were completed as required by #237 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-27 06:53:17 +0000 UTC
    </div>
</div>

