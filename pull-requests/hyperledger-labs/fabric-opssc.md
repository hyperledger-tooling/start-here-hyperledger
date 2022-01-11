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
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Add updateChannelType() and introduce the disable channel type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds the following features:
- Add `updateChannelType()` for updating the channel type to channel_ops
- Introduce 'disable' channel type to exclude the channel from management by OpsSC
  - (1) Exclude bootstrap processing for the channel in agent
  - (2) Reject a chaincode update proposal for the channel
  - (3) Allow OpsSC to manage the workflow of the proposal that has already been submitted (to prevent the control from becoming complicated)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 08:30:13 +0000 UTC
    </div>
</div>

