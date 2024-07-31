---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1241" class=".btn">#1241</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Improve prereqs logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It seems that PR #1205 has stalled, so I have created a new PR that builds upon the considerations from that one while addressing the issues raised. 

This PR resolves issue #1204 and also addresses the concerns mentioned in PR #1205. Specifically, it:
- Uses the newer install script instead of bootstrap.sh.
- Downloads binaries corresponding to the image versions, supporting both two-digit and three-digit Fabric version specifications.

Related issue:
Resolves #1204
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-31 09:42:15 +0000 UTC
    </div>
</div>

