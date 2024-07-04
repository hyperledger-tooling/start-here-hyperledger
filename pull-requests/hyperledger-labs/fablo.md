---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/460" class=".btn">#460</a>
            </td>
            <td>
                <b>
                    chore: Refactor extendChaincodesConfig.ts to allow private data in chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### References
- Original Issue: #415

#### Issue Details

The default configuration for `requiredPeerCount` causes the following error:
```
error in simulation: failed to distribute private collection, txID 123, channel 123: could not build private data dissemination plan for chaincode 123 and collection 123: required to disseminate to at least 1 peers, but know of only 0 eligible peers.
```

#### Solution

The solution is to allow `requiredPeerCount` to be set to 0. This can be achieved by modifying the logic in the code that generates this property. Specifically, removing the `|| 1` part from the following lines of code:
```javascript
const anchorPeerCountsInChannel = channel.orgs.map((o) => (o.anchorPeers || []).length);
const maxPeerCount = anchorPeerCountsInChannel.reduce((a, b) => a + b, 0);
const requiredPeerCount = anchorPeerCountsInChannel.reduce((a, b) => Math.min(a, b), maxPeerCount) || 1;
```

#### Changes Made

- Removed the `|| 1` from the calculation of `requiredPeerCount` to allow it to be set to 0 if necessary.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 01:40:25 +0000 UTC
    </div>
</div>

