---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    Fixed the version of fabric-ccenv to 2.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: ikegawa-koshi <koshi.ikegawa.mf@hitachi.com>

**What this PR does / why we need it**:

I found a bug in the current main branch and v1.0-rc2 that causes FPC to fail to build (Issue #628).
As a result of discussions with the community, it was found that it was caused by differences in the version of fabric-ccenv.
This PR solves the issue of Issue #628 by setting the version of fabric-ccenv to v2.3.0.

**Which issue(s) this PR fixes**:

Fixes #628

**Special notes for your reviewer**:

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 11:53:00 +0000 UTC
    </div>
</div>

