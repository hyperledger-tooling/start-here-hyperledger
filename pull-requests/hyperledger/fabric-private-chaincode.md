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
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/678" class=".btn">#678</a>
            </td>
            <td>
                <b>
                    Fix README.md for make docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                **What this PR does / why we need it**:

When building an FPC, we need to get the `fpc-ccenv` image, so we need to run `make docker` before running `make`.
Therefore, I changed the README.

**Which issue(s) this PR fixes**:

None

**Special notes for your reviewer**:

**Does this PR introduce a user-facing changes and/or breaks backward compatability?**:

No


Signed-off-by: ikegawa-koshi <koshi.ikegawa.mf@hitachi.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 08:20:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/677" class=".btn">#677</a>
            </td>
            <td>
                <b>
                    Updated simple-go-asset sample README with instruction on how to connect new terminal to dev-container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">comp/samples</span>
            </td>
            <td>
                
**What this PR does / why we need it**:
Added additional step in the FPC Go Simple Asset Tutorial README on how to open and connect new terminal to a running fps-development-go-support docker container. This provide clearer instruction on how to interact with the simple asset go fpc chaincode from a new terminal.

**Which issue(s) this PR fixes**:
<!--
  list existing bug, feature and/or work-item which this PR addresses.
  You might also consider creating an issue first for the PR.
-->
Fixes #676 

**Special notes for your reviewer**:

Signed-off-by: Simeon Babatunde <simeonbaba@ibm.com>
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:05:00 +0000 UTC
    </div>
</div>

