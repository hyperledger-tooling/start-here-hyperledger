---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Enhance voting functions for chaincode_ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enhances voting functions for `chaincode_ops` as follows:
- Improve voting acceptance specifications
  - Not accept overwriting of votes from the same organization
  - Not accept voting after the decision  (should explicitly raise an error)
- Support rejection of proposal
- Support withdrawal of proposal

The new `chaincode_ops` can cover a series of state transitions of chaincode update proposals,
including proposal rejection and withdrawal, although it is not yet flexible enough.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 10:43:03 +0000 UTC
    </div>
</div>

