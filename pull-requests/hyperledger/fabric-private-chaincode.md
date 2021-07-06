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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/606" class=".btn">#606</a>
            </td>
            <td>
                <b>
                    Support any chaincode name in installFPC.sh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: ikegawa-koshi <koshi.ikegawa.mf@hitachi.com>

**What this PR does / why we need it**:
When executing installFPC.sh, read the CC_ID from the environment variable to install a different chaincode than the echo.
If CC_ID is undefined, "echo" will be defined.

**Which issue(s) this PR fixes**:
N/A

**Special notes for your reviewer**:
No

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:
No

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 09:21:55 +0000 UTC
    </div>
</div>

