---
layout: default
title: fabric-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-rfcs
---

# fabric-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-rfcs/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    BFT signatures: update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The RFC currently calls for adding a gRPC service for getting the Header+Signature stream (Block attestation).

After reviewing the current (SmartBFT fabric v2.3) and proposed solution, it is clear that adding a gRPC service and multiple new proto messages needlessly duplicates code and bloats the code base. The task is realised in the current implementation by 6 lines of code - 3 in the orderer (set nil to the block payload, depending on the content type requested) and 3 in the peer (set the required content type).

We therefore revert this part of the proposal and will simply migrate the code from SmartBFT fabric v2.3 for this functionality, as described in the current RFC (see https://github.com/hyperledger/fabric-rfcs/blob/8ebea2f8fb54bdc6444229049e75eef98240cd0a/text/0010-bft-signatures.md?plain=1#L132).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 12:20:07 +0000 UTC
    </div>
</div>

